# cc-uptime

External uptime check for candycultivators.com. A GitHub Actions workflow runs every 10 minutes (and on demand) and fails if the storefront (`/us` with a body marker, `/us/es`) or the admin `/health` endpoint does not answer 200, or if the TLS certificate expires in 14 days or less. A failed run emails the repository owner (GitHub notifications, "Actions: failed workflows only"). The repo holds no secrets and nothing else; the site itself lives in a separate private repository.
