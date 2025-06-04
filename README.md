# BrowserAgent

<p align="center">
  <img src="https://browseragent.dev/logo.png" alt="BrowserAgent Logo" width="200"/>
</p>

<p align="center">
  <strong>Automate anything directly in your browser</strong>
</p>

<p align="center">
  <a href="https://browseragent.dev">Website</a> •
  <a href="#features">Features</a> •
  <a href="#installation">Installation</a> •
  <a href="#usage">Usage</a> •
  <a href="#development">Development</a> •
  <a href="#contributing">Contributing</a> •
  <a href="#license">License</a>
</p>

---

## 🚀 Overview

BrowserAgent is an open-source browser automation tool that enables you to create, deploy, and manage intelligent agents that operate directly within your browser. Whether you need to automate repetitive tasks, scrape data, or build complex workflows, BrowserAgent provides a powerful and flexible platform to accomplish your goals.

## ✨ Features

- **Browser-Native Automation**: Run automation scripts directly in your browser without external dependencies
- **Intelligent Agents**: Create sophisticated agents that can navigate websites, fill forms, extract data, and make decisions
- **Visual Builder**: Intuitive interface for creating automation workflows without coding
- **API Integration**: Connect your browser agents with external APIs and services
- **Scheduling**: Set up recurring tasks to run at specific times
- **Monitoring**: Track the performance and status of your agents in real-time
- **Collaboration**: Share and collaborate on automation projects with your team

## 📋 Requirements

- Python 3.12+
- Node.js 18+
- PostgreSQL
- Docker and Docker Compose (for development)

## 🔧 Installation

### Using Docker (Recommended)

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/BrowserAgent.git
   cd BrowserAgent
   ```

2. Copy the example environment file and configure it:
   ```bash
   cp .env.example .env
   ```
   Edit the `.env` file with your configuration details.

3. Build and start the containers:
   ```bash
   docker-compose up -d
   ```

4. Access the application:
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:8000

### Manual Installation

#### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install poetry
   poetry install
   ```

3. Run migrations:
   ```bash
   python manage.py migrate
   ```

4. Start the development server:
   ```bash
   python manage.py runserver
   ```

#### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

## 🔍 Usage

### Creating Your First Agent

1. Sign in to your BrowserAgent dashboard
2. Click "Create New Agent"
3. Choose a template or start from scratch
4. Define your agent's workflow using the visual builder
5. Test your agent in the sandbox environment
6. Deploy your agent to production

### Example Use Cases

- **Data Collection**: Automatically gather data from websites and save it to your database
- **Form Automation**: Fill out forms across multiple websites with a single click
- **Monitoring**: Keep track of price changes, stock availability, or content updates
- **Testing**: Automate browser testing for your web applications
- **Customer Service**: Build agents that can handle customer inquiries and perform actions on their behalf

## 🛠️ Development

### Project Structure

```
BrowserAgent/
├── backend/           # Django backend API
├── frontend/          # Next.js frontend application
├── nginx-conf/        # Nginx configuration for production
├── docker-compose.yml # Development Docker configuration
└── docker-compose.prod.yml # Production Docker configuration
```

### Running Tests

```bash
# Backend tests
cd backend
python manage.py test

# Frontend tests
cd frontend
npm test
```

## 🤝 Contributing

We welcome contributions to BrowserAgent! Please see our [Contributing Guide](CONTRIBUTING.md) for more details on how to get started.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Write and test your changes
4. Commit your changes (`git commit -m 'Add some amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

## 📜 License

BrowserAgent is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [Django](https://www.djangoproject.com/)
- [Next.js](https://nextjs.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [Docker](https://www.docker.com/)
- All our [contributors](https://github.com/yourusername/BrowserAgent/graphs/contributors)

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/sauravpanda">Saurav Panda</a> and <a href="https://github.com/shreyashkgupta">Shreyash Gupta</a>
</p>
