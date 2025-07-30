# Crop Prediction System

A full-stack machine learning application for crop prediction and recommendation using Django backend and React frontend.

## 🚀 Features

- **Crop Recommendation**: Get crop suggestions based on soil and climate data
- **Yield Prediction**: Predict crop yields using ML models
- **Data Visualization**: Interactive charts and graphs
- **Model Training**: Train custom ML models with your data
- **User Authentication**: Secure user management
- **Responsive Design**: Modern UI that works on all devices

## 🛠️ Tech Stack

### Backend
- **Django 5.2.7** - Web framework
- **Django REST Framework** - API development
- **scikit-learn** - Machine learning
- **pandas & numpy** - Data processing
- **xgboost** - Gradient boosting
- **SQLite** - Database (default)

### Frontend
- **React 19** - UI framework
- **TypeScript** - Type safety
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **Chart.js** - Data visualization
- **React Router** - Navigation
- **Axios** - HTTP client

## 📋 Prerequisites

- Python 3.11+
- Node.js 18+
- pnpm (recommended) or npm

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd cursor-crop-project
```

### 2. Backend Setup
```bash
# Navigate to backend directory
cd django_backend

# Create virtual environment
python -m venv backend-env

# Activate virtual environment
# On Windows:
backend-env\Scripts\activate
# On macOS/Linux:
source backend-env/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start the server
python manage.py runserver
```

The backend will be available at `http://localhost:8000`

### 3. Frontend Setup
```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

The frontend will be available at `http://localhost:5173`

## 📁 Project Structure

```
cursor-crop-project/
├── django_backend/          # Django backend
│   ├── core/               # Main app
│   ├── ml/                 # ML models and training
│   ├── data/               # Datasets and models
│   └── manage.py
├── frontend/               # React frontend
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── pages/          # Page components
│   │   ├── services/       # API services
│   │   └── utils/          # Utility functions
│   └── package.json
└── README.md
```

## 🔧 Configuration

### Environment Variables

Create `.env` files in both backend and frontend directories:

**Backend (.env in django_backend/)**
```env
DEBUG=True
SECRET_KEY=your-secret-key
ALLOWED_HOSTS=localhost,127.0.0.1
```

**Frontend (.env in frontend/)**
```env
VITE_API_URL=http://localhost:8000
```

## 📊 API Endpoints

- `POST /api/predict/` - Crop prediction
- `POST /api/train/` - Train new model
- `GET /api/models/` - List available models
- `POST /api/upload/` - Upload dataset

## 🧪 Testing

### Backend Tests
```bash
cd django_backend
pytest
```

### Frontend Tests
```bash
cd frontend
pnpm test
```

## 🚀 Deployment

See [DEPLOYMENT.md](DEPLOYMENT.md) for detailed deployment instructions.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License.

## 🆘 Support

If you encounter any issues, please create an issue in the repository. 