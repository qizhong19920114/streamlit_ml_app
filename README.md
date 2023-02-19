# streamlit_ml_app

### Run locally
- `streamlit run oAuthMain.py`

### Run locally thru Docker
- build docker `docker build -t streamlit-ml-app3-local .`
- run docker `docker run -p 8501:8501  streamlit-ml-app3-local`


### Run on GCP
- build container `gcloud builds submit --tag gcr.io/streamlit-378223/streamlit-ml-app --project=streamlit-378223`
- deploy to GCP `gcloud run deploy --image gcr.io/streamlit-378223/streamlit-ml-app2 --platform managed --project=streamlit-378223 --allow-unauthenticated`
	- this will print out a url to use


Common Issue: 
- Due to git authentication update, to clone this repo, I will need to do `git clone https://qizhong19920114:<personal_token>@github.com/qizhong19920114/streamlit_ml_app.git`
	- The "personal_token" here needs to be generated every 30 days from Setting > Developer settings > Personal access token > Tokens (classic)