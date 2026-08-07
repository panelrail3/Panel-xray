# Railway XPanel — Railway Final v1.0.2

This version fixes the Vue/Vite production build by explicitly loading
`frontend/vite.config.mjs` with the Vue plugin.

GitHub repository root must contain:

- Dockerfile
- railway.json
- entrypoint.sh
- requirements.txt
- .dockerignore
- .gitignore
- backend/
- frontend/
- alembic/

Do not wrap these files in another `railway-xpanel-final/` directory.

Railway should build the repository root with the included Dockerfile.
