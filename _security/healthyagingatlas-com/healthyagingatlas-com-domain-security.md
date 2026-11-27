---
api_specs:
- filename: healthyagingatlas-com-openapi-generated.yml
  format: yaml
  label: Healthy Aging Atlas API
  slug: healthyagingatlas-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/healthyagingatlas-com/openapi/_ae-authored/healthyagingatlas-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: healthyagingatlas.com
  spf: true
hosts:
- cert_expires: Jan  8 17:41:29 2027 GMT
  host: healthyagingatlas.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Healthy Aging Atlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Healthy Aging Atlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Healthy Aging Atlas
provider_slug: healthyagingatlas-com
slug: healthyagingatlas-com-domain-security
source_filename: healthyagingatlas-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: healthyagingatlas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 17:41:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: healthyagingatlas.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/healthyagingatlas-com/security/healthyagingatlas-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Supplements
- Evidence
- Longevity
- Nutrition
- Company
---
