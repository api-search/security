---
api_specs:
- filename: oura-oura-ring-api-openapi.yml
  format: yaml
  label: Oura Ring API
  slug: oura-ring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura/refs/heads/main/openapi/oura-oura-ring-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@ouraring.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ouraring.com
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: ouraring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: cloud.ouraring.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.ouraring.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oura Ring, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oura Ring
provider_slug: oura
slug: oura-domain-security
source_filename: oura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ouraring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.ouraring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: api.ouraring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ouraring.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@ouraring.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oura/refs/heads/main/security/oura-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Wearables
- Sleep
- Fitness
- Heart Rate
- Readiness
- Smart Ring
- Biometrics
---
