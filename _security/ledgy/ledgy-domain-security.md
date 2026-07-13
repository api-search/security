---
api_specs:
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Companies API
  slug: companies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Stakeholders API
  slug: stakeholders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Share Classes API
  slug: share-classes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy Financing Rounds API
  slug: financing-rounds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
- filename: ledgy-openapi.yml
  format: yaml
  label: Ledgy ESOP and Grants API
  slug: esop-grants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/openapi/ledgy-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ledgy.com
  spf: true
hosts:
- cert_expires: Sep 30 15:17:13 2026 GMT
  host: www.ledgy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 05:11:19 2026 GMT
  host: docs.ledgy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:38:41 2026 GMT
  host: app.ledgy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ledgy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ledgy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ledgy
provider_slug: ledgy
slug: ledgy-domain-security
source_filename: ledgy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ledgy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:17:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ledgy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:11:19 2026 GMT\n  hsts: false\n- host: app.ledgy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:38:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ledgy.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledgy/refs/heads/main/security/ledgy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Equity Management
- Cap Table
- ESOP
- Stakeholders
- GraphQL
---
