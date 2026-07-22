---
api_specs:
- filename: peakon-openapi-original.json
  format: json
  label: Peakon API
  slug: peakon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: peakon.com
  spf: true
hosts:
- cert_expires: Sep 14 04:34:11 2026 GMT
  host: www.peakon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peakon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peakon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Peakon
provider_slug: peakon
slug: peakon-domain-security
source_filename: peakon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peakon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:34:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peakon.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/security/peakon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- Employee Engagement
- Employee Experience
- HR Tech
- Surveys
- People Analytics
- Workday
---
