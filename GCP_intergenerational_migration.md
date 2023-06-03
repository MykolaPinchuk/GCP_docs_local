### This file explains which repos/projects to set up when migrating between GCP accounts for cosy minimization.

#### Resources to reset in GCP:
- GCS.
- Repos with main models in Vertex notebooks. 1-2 cheap CPU instances and 1 GPU instatnce.
- BigQuery.

The most efficient way migrate GCS data seems to be GCS transfer service. See answer #2 from https://stackoverflow.com/questions/31049535/how-can-i-move-data-directly-from-one-google-cloud-storage-project-to-another on how to enable permissions for such transfer.
See https://cloud.google.com/knowledge/kb/transfer-the-bucket-from-one-project-to-another-with-same-name-000005032 on how to do transfer after enabling permissions.

#### Notes:
- When working in two GCP accounts, open them in separate windows to use two Google accounts.
