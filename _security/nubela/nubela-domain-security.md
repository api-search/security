---
api_specs:
- filename: nubela-openapi.yml
  format: yaml
  label: Nubela Proxycurl
  slug: proxycurl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nubela/refs/heads/main/openapi/nubela-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nubela.co
  spf: true
hosts:
- cert_expires: Sep  5 17:10:06 2026 GMT
  host: nubela.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nubela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nubela, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nubela
provider_slug: nubela
slug: nubela-domain-security
source_filename: nubela-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nubela.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:10:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nubela.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nubela/refs/heads/main/security/nubela-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Companies
- Data
- People
- Scraping
---
