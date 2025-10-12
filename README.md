# Health-Guard
Heart Disease and Diabetes Prediction System

A machine learning-powered web application that predicts the likelihood of diabetes and heart disease based on user input parameters.

## Features

- **Diabetes Prediction**: Predicts diabetes based on factors like pregnancies, glucose level, blood pressure, etc.
- **Heart Disease Prediction**: Predicts heart disease based on age, gender, chest pain type, cholesterol levels, etc.
- **Interactive UI**: Built with Streamlit for an intuitive user experience
- **Machine Learning Models**: Uses trained models saved as `.sav` files

## Local Development

### Prerequisites
- Python 3.9+
- pip

### Installation
1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   streamlit run app.py
   ```

## Deployment Options

### Option 1: Netlify (Recommended for Static Hosting)

**Note**: While Netlify is primarily for static sites, Streamlit apps require serverless functions. For better Streamlit support, consider Streamlit Cloud or Heroku.

1. **Connect Repository**: Link your GitHub repository to Netlify
2. **Build Settings**:
   - Build command: `pip install -r requirements.txt && streamlit run app.py --server.port $PORT --server.address 0.0.0.0`
   - Publish directory: `.`
3. **Environment Variables**: Set `PYTHON_VERSION=3.9`
4. **Deploy**: Netlify will automatically deploy on push

### Option 2: Streamlit Cloud (Recommended)

1. Go to [share.streamlit.io](https://share.streamlit.io)
2. Connect your GitHub repository
3. Select the repository and main file (`app.py`)
4. Deploy automatically

### Option 3: Heroku

1. Install Heroku CLI
2. Create a `Procfile`:
   ```
   web: sh setup.sh && streamlit run app.py --server.port=$PORT --server.address=0.0.0.0
   ```
3. Deploy:
   ```bash
   heroku create your-app-name
   git push heroku main
   ```

## Files Structure

- `app.py` - Main Streamlit application
- `diabetes_model.sav` - Trained diabetes prediction model
- `heart_disease_model.sav` - Trained heart disease prediction model
- `diabetes.csv` - Training data for diabetes model
- `heart.csv` - Training data for heart disease model
- `requirements.txt` - Python dependencies
- `netlify.toml` - Netlify configuration
- `setup.sh` - Streamlit setup script

## Model Information

The application uses pre-trained machine learning models:
- **Diabetes Model**: Based on the Pima Indians Diabetes Database
- **Heart Disease Model**: Based on heart disease indicators

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make changes
4. Submit a pull request

## License

This project is open source and available under the MIT License.
