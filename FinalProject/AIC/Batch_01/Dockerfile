# Use an official Python runtime as a parent image
FROM python:3.10.9

# Install pip
RUN apt update && apt install -y python3-pip

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
# COPY . .

# Install any needed packages specified in requirements.txt
# RUN pip install -r ./requirements.txt

# Make port 3000 available to the world outside this container
EXPOSE 3000

# Run Jupyter Notebook
CMD ["jupyter", "notebook", "--ip=127.0.0.1", "--port=3000", "--allow-root"]