# Hacker News Newsletter

A simple newsletter service that sends you top Hacker News stories. Subscribe to get daily and weekly updates of the best content.

## Getting Started

### Backend Setup

1. Clone the repository:
\```bash
git clone https://github.com/sanjay-kandpal/frontPage-Assignment
cd hacker-news-newsletter
\```

2. Install dependencies:
\```bash
npm install
\```

3. Set up your environment variables:
\```bash
cp .env.example .env
\```

4. Update `.env` with your details:
\```env
DB_USER=your_username
DB_PASSWORD=your_password
EMAIL_USER=your_email@gmail.com
EMAIL_PASSWORD=your_app_password
\```

5. Start the server:
\```bash
npm start
\```

### Frontend Setup

1. Clone the frontend repository:
\```bash
git clone https://github.com/sanjay-kandpal/frontend-Newsletter.git
cd frontend-Newsletter
\```

2. Install dependencies:
\```bash
npm install
\```

3. Start the frontend:
\```bash
npm start
\```

## Features

- Daily news updates
- Weekly top stories digest
- Real-time story notifications
- Email subscription system

## API Examples

### Subscribe to Newsletter
\```javascript
fetch('http://localhost:3000/subscribe', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email: 'user@example.com' })
});
\```

### WebSocket Updates
\```javascript
const ws = new WebSocket('ws://localhost:8080');
ws.onmessage = (event) => {
    const data = JSON.parse(event.data);
    console.log('New stories:', data);
};
\```

## Need Help?

- Check server is running on port 3000
- Verify database connection
- Ensure Gmail credentials are correct

## Links

- [Frontend Repository](https://github.com/sanjay-kandpal/frontend-Newsletter)
- [API Documentation](./docs/api.md)
- [Contributing Guide](./CONTRIBUTING.md)