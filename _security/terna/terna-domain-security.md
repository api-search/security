---
api_specs:
- filename: terna-openapi-generated.yml
  format: yaml
  label: Terna API
  slug: terna-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terna/refs/heads/main/openapi/_ae-authored/terna-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terna.it
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: www.terna.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Terna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Terna
provider_slug: terna
slug: terna-domain-security
source_filename: terna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.terna.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: terna.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terna/refs/heads/main/security/terna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Transmission
- Infrastructure
- Italy
- Renewable
---
