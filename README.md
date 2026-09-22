# mclean.aero

Serves the Tesla Fleet API partner public key for `mclean.aero` over HTTPS at:

    /.well-known/appspecific/com.tesla.3p.public-key.pem

That file is a **public key** — it is published by design and contains nothing secret.
Tesla fetches it to verify domain ownership when registering the partner account.

Hosted on GitHub Pages deliberately, so the domain-verification endpoint adds no
attack surface to the telemetry server. See project P-036.
