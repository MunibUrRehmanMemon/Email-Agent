# Jupyter Notebook Best Practices

## 📝 Guidelines for Contributing to this Repository

### Before Committing Notebooks

1. **Clear All Outputs**: Always clear all cell outputs before committing
   ```bash
   # In Jupyter, use: Cell → All Output → Clear
   # Or programmatically clean the notebook
   ```

2. **Remove Widget State**: Remove any widget metadata that can make files large
   ```python
   # This repository includes a cleaning script for this purpose
   ```

3. **Reset Execution Counts**: Set all execution counts to `null`

### Why This Matters

- **File Size**: Notebooks with outputs can become very large (100KB+ vs 10-20KB clean)
- **Git Performance**: Large files slow down clone/pull operations
- **Merge Conflicts**: Output data creates unnecessary merge conflicts
- **Security**: Outputs might contain sensitive information

### Cleaning Script

Use the provided cleaning functionality to automatically clean notebooks:

```python
import json

def clean_notebook(input_file, output_file=None):
    if output_file is None:
        output_file = input_file
    
    with open(input_file, 'r') as f:
        nb = json.load(f)
    
    # Clean each cell
    for cell in nb['cells']:
        if 'outputs' in cell:
            cell['outputs'] = []
        if 'execution_count' in cell:
            cell['execution_count'] = None
    
    # Remove widget metadata
    if 'widgets' in nb['metadata']:
        del nb['metadata']['widgets']
    
    # Save cleaned notebook
    with open(output_file, 'w') as f:
        json.dump(nb, f, indent=2)

# Usage
clean_notebook('your_notebook.ipynb')
```

### File Size Targets

- ✅ **Good**: < 50KB (typical for clean notebooks)
- ⚠️ **Acceptable**: 50-100KB (may have some small outputs)
- ❌ **Too Large**: > 100KB (needs cleaning)

### Additional Tips

1. **Use .gitignore**: Prevent accidentally committing large files
2. **Regular Cleaning**: Clean notebooks as part of your workflow
3. **Review Before Commit**: Always check `git diff` before committing
4. **Split Large Notebooks**: Consider breaking very large notebooks into smaller ones

## 🔧 Automated Cleaning

This repository now includes automated notebook cleaning to prevent upload issues and keep the repository clean and efficient.