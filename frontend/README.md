# Frontend — [Project Name]

Put your web/mobile application here: user interfaces, dashboards, mobile apps,
PWA, etc.

## Stack (fill in)

- Framework / platform: [your choice]
- Styling: [your choice]
- HTTP client: [your choice]

## Local Setup (fill in)

```bash
cd frontend
<install frontend dependencies — command for your package manager>
<start the frontend app>
```

## Environment Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `BACKEND_URL` | Backend API base URL | `http://localhost:8000` |

> Values above are illustrative examples only — replace them with your own.
> Never commit real `.env` values — see root `.gitignore`. A starting point is
> provided in `.env.example`.

## Tests & Lint

```bash
# Replace <commands> with the ones for your stack
<your test command>
<your lint command>
<your build command>
```

## Project Layout (adjust to your stack)

```
frontend/
├── <entry point>       # app entry point
├── <root component>    # main app component
├── <components/>       # reusable UI
├── <pages/>            # route views
├── <services/>         # API calls
├── <config files for your tooling>
└── .env.example
```