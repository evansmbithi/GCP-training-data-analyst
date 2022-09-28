- Earthquake regions-ML
- git clone
- cd /courses/bdml_fundamentals/demos/earthquakevm/
- ./install_missing.sh - install dependencies
- ./ingest.sh - downloads earthquake.csv
- ./transform.py - creates a png of weekly data from earthquake.csv

- Copy the files from compute engine into cloud storage and make it public.
- Delete the VM.

- Create a bucket with a unique name
- $ gsutil ls gs://<bucket_name>
- $ gsutil cp earthquakes.* gs://<bucket_name>
- Make the storage public: Select all files > Permissions >Add Members = AllUsers
- Role: Storage Object Viewer
