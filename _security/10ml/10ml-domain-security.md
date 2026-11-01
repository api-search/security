---
api_specs:
- filename: 10ml-10ml-fragrance-index-api-openapi.yml
  format: yaml
  label: 10ML Fragrance Index API 10ML Fragrance Index API
  slug: 10ml-10ml-fragrance-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/10ml/openapi/10ml-10ml-fragrance-index-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 10ml.com
  spf: true
hosts:
- cert_expires: Dec 24 07:06:49 2026 GMT
  host: 10ml.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 10Ml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 10ML Fragrance Index API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 10ML Fragrance Index API
provider_slug: 10ml
slug: 10ml-domain-security
source_filename: 10ml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 10ml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 07:06:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 10ml.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/10ml/security/10ml-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Perfume
- Fragrance
- API
- Free
- NoAuth
---
