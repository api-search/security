---
api_specs:
- filename: the-token-company-openapi.yml
  format: yaml
  label: The Token Company Compression API
  slug: the-token-company-compression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-token-company/refs/heads/main/openapi/the-token-company-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thetokencompany.com
  spf: true
hosts:
- cert_expires: Oct  8 12:56:14 2026 GMT
  host: thetokencompany.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.thetokencompany.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Token Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Token Company, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Token Company
provider_slug: the-token-company
slug: the-token-company-domain-security
source_filename: the-token-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thetokencompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:56:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.thetokencompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: thetokencompany.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-token-company/refs/heads/main/security/the-token-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- LLM
- Artificial Intelligence
- Prompt Compression
- Tokens
- Cost Optimization
- Developer Tools
- Middleware
- API
---
