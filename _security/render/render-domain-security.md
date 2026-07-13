---
api_specs:
- filename: render-openapi.json
  format: json
  label: Render API
  slug: render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render/refs/heads/main/openapi/render-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@render.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: render.com
  spf: true
hosts:
- cert_expires: Aug 21 19:26:00 2026 GMT
  host: render.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:31:38 2026 GMT
  host: dashboard.render.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 01:57:23 2026 GMT
  host: api.render.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Render Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Render, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Render
provider_slug: render
slug: render-domain-security
source_filename: render-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: render.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:26:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.render.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:31:38 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: api.render.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:57:23 2026 GMT\n  hsts: null\ndomains:\n- domain: render.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@render.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/render/refs/heads/main/security/render-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Platform
- Deployment
- Infrastructure
- DevOps
- Web Services
- Databases
- Hosting
---
