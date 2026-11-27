---
api_specs:
- filename: manyscripts-com-openapi-generated.yml
  format: yaml
  label: ManyScripts API
  slug: manyscripts-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/manyscripts-com/openapi/_ae-authored/manyscripts-com-openapi-generated.yml
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
  dnssec: false
  domain: manyscripts.com
  spf: true
hosts:
- cert_expires: Jan 14 20:36:45 2027 GMT
  host: manyscripts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ManyScripts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ManyScripts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ManyScripts
provider_slug: manyscripts-com
slug: manyscripts-com-domain-security
source_filename: manyscripts-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manyscripts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 20:36:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: manyscripts.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/manyscripts-com/security/manyscripts-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transcription
- Video
- Artificial Intelligence
- Creator Tools
- Marketing
---
