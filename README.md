# Bill on Capitol Hill

A modern web application for tracking and analyzing legislative bills in real-time. This application provides an intuitive interface for citizens to stay informed about ongoing legislative activities.

## Features

- **Live Bill Tracking**: Real-time updates from Congress.gov API
- **Smart Summarization**: AI-powered bill analysis and categorization
- **Search & Filter**: Easy-to-use interface for finding relevant bills
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Prerequisites

- Python 3.8+
- PostgreSQL
- Node.js (for frontend development)
- Congress.gov API key
- OpenAI API key

## Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/bill-capitol-hill.git
cd bill-capitol-hill
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
```bash
cp .env.example .env
```
Edit `.env` with your actual API keys and configuration.

5. Initialize the database:
```bash
flask db init
flask db migrate
flask db upgrade
```

6. Run the application:
```bash
flask run
```

The application will be available at `http://localhost:5000`

## API Endpoints

- `GET /api/bills`: Get list of bills with optional filters
- `GET /api/bills/<bill_id>`: Get detailed information about a specific bill
- `GET /api/bills/search`: Search bills by keyword

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Congress.gov for providing the legislative data API
- OpenAI for powering the bill summarization feature 