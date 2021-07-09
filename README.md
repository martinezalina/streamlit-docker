# Streamlit One

The objective of this project is to provide an interface that allows you to select an xls, process its content and obtain the resulting xls.

## Run the app

The first time the project is used, the following commands should be run:

1. Build container:
   `docker build -f docker/Dockerfile -t streamlitapp:latest .`

2. Run container
   `docker run -d -p 8501:8501 streamlitapp:latest`

3. You can now view your Streamlit app in your browser http://localhost:8501

4. Browse to upload the xls file and select the example file located ./example/

5. Download the new file generated width the transform

6. To shut down container:
   `docker ps`
   `docker stop CONTAINER_ID`

## Additional Information

#### Stack

- Docker
- Python
- Streamlit
- Pandas
- openpyxl
- xlrd

#### Dependency documentation

- https://docs.streamlit.io/
- https://docs.streamlit.io/en/stable/streamlit_configuration.html
- https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html
