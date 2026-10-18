---
api_specs:
- filename: krosyn-connectors-api-openapi.yml
  format: yaml
  label: Chmura Software Connectors API
  slug: krosyn-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krosyn/refs/heads/main/openapi/krosyn-connectors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: krosyn.com
  spf: true
hosts:
- cert_expires: Nov 21 08:25:33 2026 GMT
  host: krosyn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Krosyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chmura Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chmura Software
provider_slug: krosyn
slug: krosyn-domain-security
source_filename: krosyn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: krosyn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 08:25:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: krosyn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/krosyn/refs/heads/main/security/krosyn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- API
- DeveloperTools
- Security
---
