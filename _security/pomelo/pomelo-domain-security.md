---
api_specs:
- filename: pomelo-authentication-api-openapi.yml
  format: yaml
  label: Pomelo Authentication API
  slug: pomelo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-authentication-api-openapi.yml
- filename: pomelo-card-accounts-api-openapi.yml
  format: yaml
  label: Pomelo Card Accounts API
  slug: pomelo-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-card-accounts-api-openapi.yml
- filename: pomelo-cards-api-openapi.yml
  format: yaml
  label: Pomelo Cards API
  slug: pomelo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-cards-api-openapi.yml
- filename: pomelo-transactions-api-openapi.yml
  format: yaml
  label: Pomelo Transactions API
  slug: pomelo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-transactions-api-openapi.yml
- filename: pomelo-transfers-api-openapi.yml
  format: yaml
  label: Pomelo Transfers API
  slug: pomelo-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-transfers-api-openapi.yml
- filename: pomelo-users-api-openapi.yml
  format: yaml
  label: Pomelo Users API
  slug: pomelo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pomelo.la
  spf: true
hosts:
- cert_expires: Sep 29 20:25:19 2026 GMT
  host: www.pomelo.la
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:25:19 2026 GMT
  host: developers.pomelo.la
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:25:19 2026 GMT
  host: api.pomelo.la
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pomelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pomelo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Pomelo
provider_slug: pomelo
slug: pomelo-domain-security
source_filename: pomelo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pomelo.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.pomelo.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pomelo.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pomelo.la\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/security/pomelo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fintech
- Card Issuing
- Embedded Finance
- Payments
- Latin America
---
