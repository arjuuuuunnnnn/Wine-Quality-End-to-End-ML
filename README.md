## An End-to-End machine learning project with Flask

### Dockerized
```bash
docker pull arjuuuuunnnnn/wine-quality-ml:1
```
### Deployed in AZURE cloud [https://wine-quality-ml-hemanth.azurewebsites.net/](https://wine-quality-ml-hemanth.azurewebsites.net/)

- Data ingestion (from google drive link reading and loading the dataset into the project)
- Data Validation
- Data transformation
- Training the model
- Evaluation of the model

## Usage:
```bash
pip install -r requirements.txt
```
```bash
python app.py
```
Then go to the redirected browser.

## Modify and Use
- To change the dataset - Go to `config/config.yaml` file and change the ```source_url``` variable
- To change the attributes and their types - Go to `schema.yaml` file and change the ```COLUMNS``` and ```TARGET_COLUMN``` variables
- To change the parameters for the model - Go to `params.yaml` file and change them
- If there requires more data preprocessing, add that in the file `src/mlProject/components/data_transformation.py`
- To change the model - Go to `src/mlProject/components/model_trainer.py` and change to the required model

## Workflow
- update config.yaml
- update schema.yaml
- update params.yaml
- update the entity
- update the configuration manager in src config
- update the components
- update the pipeline
- update the main.py
- At last update the app.py

#### By running `main.py`
```bash
python main.py
```
All the information of the project from data ingestion to prediction is saved in the file `logs/running_logs.log`


### DVC has to be implemented and working on it..