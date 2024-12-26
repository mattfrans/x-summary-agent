# X Summary Agent

A Python-based AI agent that fetches tweets from your X (formerly Twitter) timeline and generates concise summaries using the T5 transformer model.

## Features

- Fetches recent posts from your X timeline
- Generates AI-powered summaries using the T5 transformer model
- Saves summaries to JSON for further analysis
- Environment-based configuration for secure credential management

## Prerequisites

- Python 3.12+
- Twitter Developer Account with API credentials
- Required Python packages (see `requirements.txt`)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/mattfrans/x-summary-agent.git
cd x-summary-agent
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
# On Windows
.\venv\Scripts\activate
# On Unix or MacOS
source venv/bin/activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the root directory with your X API credentials:
```env
CONSUMER_KEY=your_consumer_key
CONSUMER_SECRET=your_consumer_secret
ACCESS_TOKEN=your_access_token
ACCESS_TOKEN_SECRET=your_access_token_secret
```

## Usage

Run the agent:
```bash
python x_agent.py
```

The script will:
1. Fetch recent posts from your timeline
2. Generate summaries using the T5 model
3. Display summaries in the console
4. Save summaries to `my_timeline_summaries.json`

## Dependencies

- tweepy - X/Twitter API interaction
- transformers - Text summarization using T5
- python-dotenv - Environment variable management
- torch - Required for transformers

## License

MIT License

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
