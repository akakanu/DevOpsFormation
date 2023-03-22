# Install the base requirements for the app.
FROM python:2.7-stretch
# Maintainer of image.
LABEL maintainer="akakanu (alexisndorama@yahoo.ca)" 
# Copy SOURCE CODE in the image .
ADD student_age.py /
# Install of dependencies
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0ip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0
# Create the Data Folder
VOLUME ["/data"]
# Expose port
EXPOSE 5000
# Run code
CMD ["python", "./student_age.py"]
