<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Email Agent - README</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css">
    <style>
        .readme-container {
            max-width: 1000px;
            margin: 0 auto;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Helvetica', 'Arial', sans-serif;
        }
        .code-block {
            background-color: #f6f8fa;
            border: 1px solid #d1d9e0;
            border-radius: 6px;
            color: #24292f;
            font-family: ui-monospace, SFMono-Regular, 'SF Mono', Consolas, 'Liberation Mono', Menlo, monospace;
            font-size: 12px;
            line-height: 1.45;
            overflow: auto;
            padding: 16px;
            white-space: pre;
        }
        .inline-code {
            background-color: rgba(175, 184, 193, 0.2);
            border-radius: 6px;
            font-family: ui-monospace, SFMono-Regular, 'SF Mono', Consolas, 'Liberation Mono', Menlo, monospace;
            font-size: 85%;
            padding: 0.2em 0.4em;
        }
        .warning-box {
            background-color: #fff8dc;
            border-left: 4px solid #f0ad4e;
            padding: 12px 16px;
            margin: 16px 0;
            border-radius: 4px;
        }
        .danger-box {
            background-color: #fdf2f2;
            border-left: 4px solid #dc3545;
            padding: 12px 16px;
            margin: 16px 0;
            border-radius: 4px;
        }
        .info-box {
            background-color: #e7f3ff;
            border-left: 4px solid #0969da;
            padding: 12px 16px;
            margin: 16px 0;
            border-radius: 4px;
        }
        .success-box {
            background-color: #f0fff4;
            border-left: 4px solid #28a745;
            padding: 12px 16px;
            margin: 16px 0;
            border-radius: 4px;
        }
        .feature-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 12px;
            padding: 20px;
            margin: 12px 0;
            color: white;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }
        .tech-badge {
            display: inline-block;
            background: linear-gradient(45deg, #4285f4, #34a853);
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
            margin: 2px 4px;
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <div class="readme-container px-4 py-8">
        <!-- Header -->
        <div class="text-center mb-12">
            <h1 class="text-5xl font-bold mb-4 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
                <i class="fas fa-robot mr-3"></i>AI Email Agent
            </h1>
            <p class="text-xl text-gray-600 mb-6">
                Intelligent email automation powered by <strong>Gemma 3n E4B</strong> for personalized outreach
            </p>
            
            <!-- Badges -->
            <div class="flex flex-wrap justify-center gap-2 mb-6">
                <span class="tech-badge"><i class="fas fa-brain mr-1"></i>Gemma 3n E4B</span>
                <span class="tech-badge"><i class="fab fa-python mr-1"></i>Python 3.8+</span>
                <span class="tech-badge"><i class="fas fa-envelope mr-1"></i>Gmail API</span>
                <span class="tech-badge"><i class="fas fa-spider mr-1"></i>Web Scraping</span>
                <span class="tech-badge"><i class="fab fa-google mr-1"></i>Google Colab</span>
            </div>
        </div>

        <!-- Quick Navigation -->
        <div class="bg-gray-50 rounded-lg p-6 mb-8">
            <h3 class="text-lg font-semibold mb-4"><i class="fas fa-compass mr-2"></i>Quick Navigation</h3>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <a href="#features" class="text-blue-600 hover:text-blue-800 flex items-center">
                    <i class="fas fa-star mr-2"></i>Features
                </a>
                <a href="#installation" class="text-blue-600 hover:text-blue-800 flex items-center">
                    <i class="fas fa-download mr-2"></i>Installation
                </a>
                <a href="#usage" class="text-blue-600 hover:text-blue-800 flex items-center">
                    <i class="fas fa-play mr-2"></i>Usage
                </a>
                <a href="#ethics" class="text-blue-600 hover:text-blue-800 flex items-center">
                    <i class="fas fa-balance-scale mr-2"></i>Ethics
                </a>
            </div>
        </div>

        <!-- Description -->
        <div class="mb-8">
            <h2 class="text-3xl font-bold mb-4"><i class="fas fa-info-circle mr-2 text-blue-600"></i>Overview</h2>
            <p class="text-lg text-gray-700 leading-relaxed mb-4">
                This AI-powered email agent automates the process of researching companies and crafting personalized outreach emails. 
                Built for Google Colab, it combines web scraping, AI text generation using <strong>Gemma 3n E4B</strong>, and Gmail API integration 
                to create a comprehensive email automation solution.
            </p>
            
            <div class="info-box">
                <p><i class="fas fa-lightbulb mr-2 text-blue-600"></i><strong>Perfect for:</strong> Job seekers, business development professionals, researchers, and anyone needing intelligent email outreach with proper personalization.</p>
            </div>
        </div>

        <!-- Features -->
        <div id="features" class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-star mr-2 text-yellow-500"></i>Key Features</h2>
            
            <div class="grid md:grid-cols-2 gap-6">
                <div class="feature-card">
                    <div class="flex items-center mb-3">
                        <i class="fas fa-brain text-2xl mr-3"></i>
                        <h3 class="text-xl font-semibold">AI-Powered Email Generation</h3>
                    </div>
                    <p>Uses Google's Gemma 3n E4B model to create highly personalized, contextual emails based on company research and your profile.</p>
                </div>

                <div class="feature-card">
                    <div class="flex items-center mb-3">
                        <i class="fas fa-spider text-2xl mr-3"></i>
                        <h3 class="text-xl font-semibold">Intelligent Web Scraping</h3>
                    </div>
                    <p>Automatically extracts company information, email addresses, and context from websites with ethical rate limiting.</p>
                </div>

                <div class="feature-card">
                    <div class="flex items-center mb-3">
                        <i class="fas fa-envelope text-2xl mr-3"></i>
                        <h3 class="text-xl font-semibold">Gmail Integration</h3>
                    </div>
                    <p>Seamlessly sends emails through Gmail API with proper authentication and tracking capabilities.</p>
                </div>

                <div class="feature-card">
                    <div class="flex items-center mb-3">
                        <i class="fas fa-shield-alt text-2xl mr-3"></i>
                        <h3 class="text-xl font-semibold">Ethical Practices</h3>
                    </div>
                    <p>Built-in rate limiting, robots.txt respect, and preview mode to ensure responsible usage.</p>
                </div>
            </div>

            <div class="mt-6">
                <h3 class="text-xl font-semibold mb-4">Additional Capabilities:</h3>
                <div class="grid md:grid-cols-3 gap-4">
                    <div class="bg-gray-50 p-4 rounded-lg">
                        <i class="fas fa-search text-blue-600 mb-2"></i>
                        <p><strong>Email Discovery:</strong> Finds contact emails from company websites</p>
                    </div>
                    <div class="bg-gray-50 p-4 rounded-lg">
                        <i class="fas fa-chart-line text-green-600 mb-2"></i>
                        <p><strong>Campaign Tracking:</strong> Monitors sent emails and success rates</p>
                    </div>
                    <div class="bg-gray-50 p-4 rounded-lg">
                        <i class="fas fa-file-export text-purple-600 mb-2"></i>
                        <p><strong>Export Results:</strong> Save campaign data in JSON format</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Installation -->
        <div id="installation" class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-download mr-2 text-green-600"></i>Installation & Setup</h2>
            
            <div class="warning-box">
                <p><i class="fas fa-exclamation-triangle mr-2"></i><strong>Important:</strong> This project is designed to run in Google Colab for optimal GPU support and ease of setup.</p>
            </div>

            <h3 class="text-xl font-semibold mb-4">1. Prerequisites</h3>
            <ul class="list-disc pl-6 mb-6 space-y-2">
                <li><strong>Google Account:</strong> For Colab access and Gmail API</li>
                <li><strong>Hugging Face Account:</strong> For Gemma 3n E4B access</li>
                <li><strong>Gmail OAuth2 Credentials:</strong> For email sending capability</li>
            </ul>

            <h3 class="text-xl font-semibold mb-4">2. Google Colab Setup</h3>
            <div class="code-block mb-4">
# Clone the repository
!git clone https://github.com/yourusername/ai-email-agent.git
%cd ai-email-agent

# Install dependencies (automatically handled in notebook)
!pip install beautifulsoup4 requests fake-useragent tldextract
!pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client
!pip install transformers torch accelerate huggingface_hub
            </div>

            <h3 class="text-xl font-semibold mb-4">3. API Keys Configuration</h3>
            <div class="space-y-4">
                <div>
                    <h4 class="font-semibold mb-2"><i class="fab fa-google mr-2"></i>Hugging Face Setup:</h4>
                    <ol class="list-decimal pl-6 space-y-2">
                        <li>Create account at <a href="https://huggingface.co" class="text-blue-600 hover:underline">huggingface.co</a></li>
                        <li>Generate API token in Settings → Access Tokens</li>
                        <li>Add token to Colab Secrets with key <span class="inline-code">HF_TOKEN</span></li>
                    </ol>
                </div>

                <div>
                    <h4 class="font-semibold mb-2"><i class="fas fa-envelope mr-2"></i>Gmail API Setup:</h4>
                    <ol class="list-decimal pl-6 space-y-2">
                        <li>Go to <a href="https://console.cloud.google.com" class="text-blue-600 hover:underline">Google Cloud Console</a></li>
                        <li>Create new project or select existing one</li>
                        <li>Enable Gmail API</li>
                        <li>Create OAuth2 credentials (Desktop Application)</li>
                        <li>Download credentials JSON file</li>
                        <li>Upload to Colab files</li>
                    </ol>
                </div>
            </div>
        </div>

        <!-- Usage -->
        <div id="usage" class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-play mr-2 text-blue-600"></i>Usage Guide</h2>

            <h3 class="text-xl font-semibold mb-4">1. Configure Your Profile</h3>
            <div class="code-block mb-4">
my_profile = PersonalProfile(
    name="Your Name",
    email="your.email@gmail.com",
    linkedin="linkedin.com/in/yourprofile",
    github="github.com/yourusername",
    skills=["Python", "Machine Learning", "AI", "Data Science"],
    projects=[
        "AI Chatbot using LLMs",
        "Computer Vision Application",
        "Data Analysis Dashboard"
    ],
    achievements=[
        "Winner at AI Hackathon",
        "Published research paper",
        "Led ML team at startup"
    ],
    goal="Find AI/ML engineering role at innovative tech company"
)
            </div>

            <h3 class="text-xl font-semibold mb-4">2. Define Target Companies</h3>
            <div class="code-block mb-4">
target_companies = {
    "OpenAI": "https://openai.com/careers",
    "Anthropic": "https://www.anthropic.com/careers",
    "Hugging Face": "https://huggingface.co/careers",
    "Your Target Company": "https://company-website.com"
}
            </div>

            <h3 class="text-xl font-semibold mb-4">3. Run the Agent</h3>
            <div class="code-block mb-4">
# Initialize agent
agent = EmailAgent(profile=my_profile)

# Process companies (preview mode)
results = agent.process_companies(
    companies=target_companies,
    send_emails=False  # Set to True to actually send
)

# Review generated emails
print(agent.get_summary())

# Send emails (optional)
# send_results = agent.send_generated_emails()
            </div>

            <h3 class="text-xl font-semibold mb-4">4. Example Output</h3>
            <div class="bg-gray-50 p-4 rounded-lg">
                <p class="font-semibold mb-2">Generated Email Example:</p>
                <div class="bg-white p-4 border-l-4 border-blue-500 rounded">
                    <p><strong>Subject:</strong> AI Engineer interested in OpenAI's innovative work</p>
                    <p class="mt-2"><strong>Body:</strong></p>
                    <p class="mt-1 text-gray-700">Dear OpenAI Team,</p>
                    <p class="mt-1 text-gray-700">I'm [Your Name], an AI engineer with expertise in Machine Learning and Computer Vision. I've been following OpenAI's groundbreaking work in large language models...</p>
                </div>
            </div>
        </div>

        <!-- Ethics & Legal -->
        <div id="ethics" class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-balance-scale mr-2 text-red-600"></i>Ethical Guidelines & Legal Considerations</h2>
            
            <div class="danger-box">
                <h3 class="font-bold text-red-800 mb-2"><i class="fas fa-exclamation-triangle mr-2"></i>IMPORTANT DISCLAIMERS</h3>
                <p>This tool is designed for legitimate professional outreach only. Users are responsible for ensuring compliance with all applicable laws and regulations.</p>
            </div>

            <div class="grid md:grid-cols-2 gap-6">
                <div class="bg-red-50 p-6 rounded-lg border border-red-200">
                    <h3 class="font-bold text-red-800 mb-3"><i class="fas fa-ban mr-2"></i>DO NOT USE FOR:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-red-700">
                        <li>Spam or unsolicited bulk email</li>
                        <li>Harassment or repeated unwanted contact</li>
                        <li>Fraudulent or deceptive practices</li>
                        <li>Violation of website terms of service</li>
                        <li>GDPR/privacy law violations</li>
                    </ul>
                </div>

                <div class="bg-green-50 p-6 rounded-lg border border-green-200">
                    <h3 class="font-bold text-green-800 mb-3"><i class="fas fa-check mr-2"></i>PROPER USAGE:</h3>
                    <ul class="list-disc pl-6 space-y-1 text-green-700">
                        <li>Professional networking and job seeking</li>
                        <li>Business development (B2B only)</li>
                        <li>Research collaboration inquiries</li>
                        <li>Respectful, one-time outreach</li>
                        <li>Following up on existing connections</li>
                    </ul>
                </div>
            </div>

            <h3 class="text-xl font-semibold mb-4 mt-6">Built-in Ethical Features:</h3>
            <div class="grid md:grid-cols-3 gap-4">
                <div class="bg-blue-50 p-4 rounded-lg">
                    <i class="fas fa-clock text-blue-600 mb-2"></i>
                    <p><strong>Rate Limiting:</strong> 2-4 second delays between requests</p>
                </div>
                <div class="bg-blue-50 p-4 rounded-lg">
                    <i class="fas fa-robot text-blue-600 mb-2"></i>
                    <p><strong>Robots.txt:</strong> Respects website crawling policies</p>
                </div>
                <div class="bg-blue-50 p-4 rounded-lg">
                    <i class="fas fa-eye text-blue-600 mb-2"></i>
                    <p><strong>Preview Mode:</strong> Review before sending</p>
                </div>
            </div>

            <div class="warning-box mt-6">
                <p><i class="fas fa-gavel mr-2"></i><strong>Legal Compliance:</strong> Ensure compliance with CAN-SPAM Act, GDPR, and other applicable regulations in your jurisdiction. Always provide clear unsubscribe options and respect opt-out requests.</p>
            </div>
        </div>

        <!-- File Structure -->
        <div class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-folder mr-2 text-yellow-600"></i>Project Structure</h2>
            <div class="code-block">
ai-email-agent/
├── email_agent_updated.py          # Main notebook/script
├── README.md                       # This documentation
├── requirements.txt                # Python dependencies
├── credentials/                    # Store API credentials (gitignored)
│   ├── gmail_credentials.json
│   └── .env
├── exports/                        # Campaign results
│   └── email_campaign_*.json
├── examples/                       # Usage examples
│   ├── basic_usage.py
│   └── advanced_configuration.py
└── .gitignore                      # Git ignore file
            </div>
        </div>

        <!-- Configuration -->
        <div class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-cog mr-2 text-gray-600"></i>Advanced Configuration</h2>
            
            <h3 class="text-xl font-semibold mb-4">Email Generation Parameters</h3>
            <div class="code-block mb-4">
# Customize Gemma 3n generation parameters
generation_config = {
    "max_new_tokens": 400,
    "temperature": 0.7,       # Creativity level (0.1-1.0)
    "top_p": 0.9,            # Nucleus sampling
    "do_sample": True        # Enable sampling
}
            </div>

            <h3 class="text-xl font-semibold mb-4">Scraping Configuration</h3>
            <div class="code-block mb-4">
# Adjust scraping behavior
scraper_config = {
    "min_delay": 2,           # Seconds between requests
    "max_emails": 5,          # Max emails per company
    "timeout": 15,            # Request timeout
    "max_retries": 3          # Retry failed requests
}
            </div>
        </div>

        <!-- Troubleshooting -->
        <div class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-wrench mr-2 text-orange-600"></i>Troubleshooting</h2>
            
            <div class="space-y-4">
                <div class="bg-gray-50 p-4 rounded-lg">
                    <h3 class="font-semibold mb-2"><i class="fas fa-exclamation-circle mr-2 text-red-600"></i>Common Issues:</h3>
                    <ul class="list-disc pl-6 space-y-2">
                        <li><strong>GPU Out of Memory:</strong> Restart runtime, use smaller batch sizes</li>
                        <li><strong>Gmail Authentication Failed:</strong> Check OAuth2 credentials and scopes</li>
                        <li><strong>Model Loading Error:</strong> Verify HuggingFace token and model access</li>
                        <li><strong>Scraping Blocked:</strong> Some sites block automated access - this is normal</li>
                    </ul>
                </div>

                <div class="info-box">
                    <p><i class="fas fa-lightbulb mr-2"></i><strong>Performance Tips:</strong> Use T4 or better GPU in Colab, enable High-RAM mode if available, and consider using smaller model variants for faster inference.</p>
                </div>
            </div>
        </div>

        <!-- Contributing -->
        <div class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-hands-helping mr-2 text-purple-600"></i>Contributing</h2>
            <p class="mb-4">Contributions are welcome! Please follow these guidelines:</p>
            
            <div class="space-y-4">
                <div>
                    <h3 class="font-semibold mb-2">How to Contribute:</h3>
                    <ol class="list-decimal pl-6 space-y-2">
                        <li>Fork the repository</li>
                        <li>Create a feature branch (<span class="inline-code">git checkout -b feature/amazing-feature</span>)</li>
                        <li>Commit your changes (<span class="inline-code">git commit -m 'Add amazing feature'</span>)</li>
                        <li>Push to the branch (<span class="inline-code">git push origin feature/amazing-feature</span>)</li>
                        <li>Open a Pull Request</li>
                    </ol>
                </div>

                <div>
                    <h3 class="font-semibold mb-2">Areas for Contribution:</h3>
                    <ul class="list-disc pl-6 space-y-1">
                        <li>Additional AI models integration (Claude, GPT-4, etc.)</li>
                        <li>Enhanced web scraping capabilities</li>
                        <li>Email template customization</li>
                        <li>Better error handling and logging</li>
                        <li>Documentation improvements</li>
                        <li>Test coverage</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- License -->
        <div class="mb-8">
            <h2 class="text-3xl font-bold mb-6"><i class="fas fa-certificate mr-2 text-indigo-600"></i>License & Acknowledgments</h2>
            
            <div class="bg-gray-50 p-6 rounded-lg">
                <h3 class="font-semibold mb-4">License</h3>
                <p class="mb-4">This project is licensed under the MIT License - see the LICENSE file for details.</p>
                
                <h3 class="font-semibold mb-4">Acknowledgments</h3>
                <ul class="list-disc pl-6 space-y-1">
                    <li><strong>Google:</strong> For Gemma 3n E4B model and Colab platform</li>
                    <li><strong>Hugging Face:</strong> For model hosting and transformers library</li>
                    <li><strong>Gmail API:</strong> For email sending capabilities</li>
                    <li><strong>Open Source Community:</strong> For the various libraries used</li>
                </ul>
            </div>
        </div>

        <!-- Contact -->
        <div class="text-center bg-gradient-to-r from-blue-600 to-purple-600 text-white p-8 rounded-lg">
            <h2 class="text-2xl font-bold mb-4">Questions or Suggestions?</h2>
            <p class="mb-4">Feel free to reach out for support or collaboration!</p>
            <div class="flex justify-center space-x-6">
                <a href="mailto:munibmemon22@gmail.com" class="text-white hover:text-blue-200">
                    <i class="fas fa-envelope text-xl"></i> Email
                </a>
                <a href="https://linkedin.com/in/muniburrehman-memon-499862234" class="text-white hover:text-blue-200">
                    <i class="fab fa-linkedin text-xl"></i> LinkedIn
                </a>
                <a href="https://github.com/MunibUrRehmanMemon" class="text-white hover:text-blue-200">
                    <i class="fab fa-github text-xl"></i> GitHub
                </a>
            </div>
        </div>

        <!-- Footer -->
        <div class="text-center mt-8 pt-8 border-t border-gray-200">
            <p class="text-gray-600">
                Made with <i class="fas fa-heart text-red-500"></i> by Munib Ur Rehman Memon | 
                <span class="inline-code">AI Email Agent v1.0</span>
            </p>
        </div>
    </div>
</body>
</html>

