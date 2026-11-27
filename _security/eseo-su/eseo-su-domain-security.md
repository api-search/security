---
api_specs:
- filename: eseo-su-openapi.yml
  format: yaml
  label: ESEO Public API
  slug: eseo-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eseo-su/openapi/eseo-su-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eseo.su
  spf: true
hosts:
- cert_expires: Jan 10 18:40:50 2027 GMT
  host: eseo.su
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ESEO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ESEO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ESEO
provider_slug: eseo-su
slug: eseo-su-domain-security
source_filename: eseo-su-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eseo.su\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 18:40:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eseo.su\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eseo-su/security/eseo-su-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- E-Commerce
- SEO
- Marketplace
- Automation
- Company
---
