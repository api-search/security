---
api_specs:
- filename: scotiabank-tranxact-openapi.yml
  format: yaml
  label: Scotia TranXact APIs
  slug: scotia-tranxact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-tranxact-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scotiabank.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: developer.scotiabank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: developer.api.scotiabank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scotiabank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scotiabank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scotiabank
provider_slug: scotiabank
slug: scotiabank-domain-security
source_filename: scotiabank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.scotiabank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.api.scotiabank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scotiabank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/security/scotiabank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Finance
- Payments
- Canada
- Open Banking
---
