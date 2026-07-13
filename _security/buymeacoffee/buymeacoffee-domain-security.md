---
api_specs:
- filename: buymeacoffee-openapi.yml
  format: yaml
  label: Buy Me a Coffee Supporters API
  slug: buymeacoffee-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/openapi/buymeacoffee-openapi.yml
- filename: buymeacoffee-openapi.yml
  format: yaml
  label: Buy Me a Coffee Subscriptions API
  slug: buymeacoffee-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/openapi/buymeacoffee-openapi.yml
- filename: buymeacoffee-openapi.yml
  format: yaml
  label: Buy Me a Coffee Extras API
  slug: buymeacoffee-extras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/openapi/buymeacoffee-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buymeacoffee.com
  spf: true
hosts:
- cert_expires: Sep  6 22:17:32 2026 GMT
  host: www.buymeacoffee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:17:32 2026 GMT
  host: developers.buymeacoffee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:17:32 2026 GMT
  host: help.buymeacoffee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buymeacoffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buy Me a Coffee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Buy Me a Coffee
provider_slug: buymeacoffee
slug: buymeacoffee-domain-security
source_filename: buymeacoffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buymeacoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:17:32 2026 GMT\n  hsts: false\n- host: developers.buymeacoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:17:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.buymeacoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:17:32 2026 GMT\n  hsts: false\ndomains:\n- domain: buymeacoffee.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buymeacoffee/refs/heads/main/security/buymeacoffee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creator Economy
- Memberships
- Subscriptions
- Tips
- Payments
- Donations
---
