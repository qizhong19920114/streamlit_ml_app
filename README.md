# streamlit_ml_app

### run locally
- `streamlit run oAuthMain.py`

### run locally thru Docker
- build docker `docker build -t streamlit-ml-app3-local .`
- run docker `docker run -p 8501:8501  streamlit-ml-app3-local`


### run from GCP
- build container `gcloud builds submit --tag gcr.io/streamlit-378223/streamlit-ml-app --project=streamlit-378223`
- deploy to GCP `gcloud run deploy --image gcr.io/streamlit-378223/streamlit-ml-app2 --platform managed --project=streamlit-378223 --allow-unauthenticated`
	- this will print out a url to use

