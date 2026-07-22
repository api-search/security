---
api_specs:
- filename: preply-openapi-original.json
  format: json
  label: Preply Plugin API
  slug: preply-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preply/refs/heads/main/openapi/preply-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: preply.com
  spf: true
hosts:
- cert_expires: Aug 27 09:52:32 2026 GMT
  host: preply.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Preply
provider_slug: preply
slug: preply-domain-security
source_filename: preply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: preply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:52:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: preply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preply/refs/heads/main/security/preply-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Language Learning
- Tutoring
- Marketplace
- EdTech
- Search
---
