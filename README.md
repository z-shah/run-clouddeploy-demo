# Skaffold + Cloud Build + Cloud Deploy demo


- This example does not create the two cloud run services (`hello-dev` and `hello-prod` ). You will need to create them first.

- Refer `build-trigger.yaml` for substition variables required for the Cloud build trigger.

- Apply cloud deploy config after creating the two cloud run services.


## **Set env variables and create cloud deploy pipeline**

```

PROJECT_ID=
REGION=
gcloud deploy apply --file=./clouddeploy.yaml --region=$REGION --project=$PROJECT_ID

```

