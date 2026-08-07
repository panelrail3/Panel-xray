# Railway XPanel — Railway Final v1.0.1

This archive is normalized for deployment from the repository root.

## GitHub repository layout

The contents of this archive must be placed directly in the GitHub repository root:

- Dockerfile
- railway.json
- entrypoint.sh
- requirements.txt
- .dockerignore
- .gitignore
- backend/
- frontend/
- alembic/

Do NOT put the `railway-xpanel-final` directory around these files.

## Railway

Set the service Root Directory to `/` (repository root) unless your Railway project uses another explicit source directory.

The Dockerfile is intended to be selected automatically by Railway's Dockerfile builder.

## Build

The Dockerfile uses:

- Node 22 Alpine for the frontend build
- Python 3.12 slim for the application
- Xray-core 26.6.1

The frontend is compiled and its `dist` output is copied into the Python application image.
