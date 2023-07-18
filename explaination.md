# Yolo Kubernetes Orchestration

## Choice of Objects Used

This project utilizes deployment, services, config maps, and persistent volume. The files are separated into the backend and the client directory for efficiency.

The services for both client and backend are set to ensure that they are exposed externally.

## Storage solutions

The project uses a local Mongo DB connection and a persistent volume size of 1Gi. This volume is linked to the backend deployment since they are interdependent. The config map stores the DB URL to the local Mongo DB.

## Git workflow

The K8 files are version-controlled using Git alongside other project files, and changes are be committed and pushed to a Git repository.

