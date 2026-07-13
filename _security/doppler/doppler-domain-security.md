---
api_specs:
- filename: doppler-openapi.yml
  format: yaml
  label: Doppler REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppler/refs/heads/main/openapi/doppler-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doppler.com
  spf: true
hosts:
- cert_expires: Aug 26 10:36:07 2026 GMT
  host: www.doppler.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:27:28 2026 GMT
  host: docs.doppler.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:48:42 2026 GMT
  host: api.doppler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doppler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doppler, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Doppler
provider_slug: doppler
slug: doppler-domain-security
source_filename: doppler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doppler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 10:36:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.doppler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:27:28 2026 GMT\n  hsts: null\n- host: api.doppler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:48:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doppler.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doppler/refs/heads/main/security/doppler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Secrets Management
- SecretOps
- DevOps
- Configuration Management
- Security
- CI/CD
---
