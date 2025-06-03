# Gramps Web API

This is the repository for **Gramps Web API**, a Python REST API for [Gramps](https://gramps-project.org).

It allows to query and manipulate a [Gramps](https://gramps-project.org) family tree database via the web.

Gramps Web API is the backend of [Gramps Web](https://www.grampsweb.org/), a genealogy web app based on Gramps, but can also be used as backend for other tools.

## More information

- API documentation for Gramps Web API: https://gramps-project.github.io/gramps-web-api/
- Developer documentation for Gramps Web API: https://www.grampsweb.org/dev-backend/
- Documentation for Gramps Web: https://www.grampsweb.org

## Related projects

- Gramps Web frontend repository: https://github.com/gramps-project/gramps-web


## OIDC Login (Backend Only)

This backend-only implementation adds OpenID Connect (OIDC) login via Google, GitHub, and Microsoft using [Authlib](https://docs.authlib.org).

### Features
- Role-based login with Google, GitHub, Microsoft
- Backend-only logic (no frontend UI changes)
- Session-based user info (not persisted in DB)

### Setup Instructions

1. Install dependencies

```bash
pip install Authlib python-dotenv

```

2. Copy and fill your .env file

```bash
cp .env.example .env
```

3. Update .env with your OIDC client IDs and secrets

4. Run the app

5. Login

Visit:

    http://localhost:5000/auth/login/google

    http://localhost:5000/auth/login/github

    http://localhost:5000/auth/login/microsoft