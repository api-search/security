---
api_specs:
- filename: thundercompute-openapi.yml
  format: yaml
  label: Thunder Compute Instances API
  slug: thundercompute-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-openapi.yml
- filename: thundercompute-openapi.yml
  format: yaml
  label: Thunder Compute Snapshots API
  slug: thundercompute-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-openapi.yml
- filename: thundercompute-openapi.yml
  format: yaml
  label: Thunder Compute Account API
  slug: thundercompute-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thundercompute.com
  spf: true
hosts:
- cert_expires: Sep 23 23:47:51 2026 GMT
  host: www.thundercompute.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 20:28:17 2026 GMT
  host: api.thundercompute.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thundercompute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thunder Compute, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Thunder Compute
provider_slug: thundercompute
slug: thundercompute-domain-security
source_filename: thundercompute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thundercompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.thundercompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:28:17 2026 GMT\n  hsts: null\ndomains:\n- domain: thundercompute.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/security/thundercompute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GPU
- Cloud
- Infrastructure
- AI
- Compute
---
