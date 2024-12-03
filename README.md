# firstproject
## MLOPs end-to-end project
Kaggle Competition: Data from [link](https://www.kaggle.com/competitions/playground-series-s3e8/data?select=sample_submission.csv)

<font color='red'>
Sunny stopped pushing at some point, so I put some codes from his other repos. The final result might not be a running code, but the structure of files for MLOPs frameworks are correct.
When is fully working and up-to-date if it exists:

- MLflow
- Docker
- Airflow
- DVC
**As far as I remember, the only thing not running is the continuous training scripts (not related to Airflow).**
</font>
## Code

```bash
conda activate ./env
python src/pipeline/training_pipeline.py
mlflow ui
mkdir airflow
mkdir airflow/dags
touch airflow/dags/batch_prediction.py
touch airflow/dags/training_pipeline.py
docker-compose up
touch dvc.yaml
code  dvc.yaml
ls Dockerfile
touch  Dockerfile.airflow
code  Dockerfile.airflow
touch start.sh
code start.sh
touch docker-compose.yaml
code  docker-compose.yaml
docker images
touch .dockerignore
code .dockerignore
docker-compose up
docker-compose up
touch Dockerfile.flask
code  Dockerfile.flask
docker-compose up
airflow db init    # inistialize the database, but I don't remember it was necessary in this project, still sunny used it maybe for illustration.
docker compose up
```