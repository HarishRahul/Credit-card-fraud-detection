FROM python:3.8

# Set working directory
WORKDIR /app

# Install Altair with specific version
RUN pip install altair==4.1.0

# Copy requirements file
COPY ./requirements.txt /app/requirements.txt

# Install Python dependencies
RUN pip install -r requirements.txt

# Copy the rest of the application code
COPY . /app

# Command to run the Streamlit app
CMD ["streamlit", "run", "app.py"]
