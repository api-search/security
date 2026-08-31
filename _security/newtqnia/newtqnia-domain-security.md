---
api_specs:
- filename: newtqnia-news-api-openapi.yml
  format: yaml
  label: NewTqnia | Technology News, AI and Innovation News API
  slug: newtqnia-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newtqnia/refs/heads/main/openapi/newtqnia-news-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newtqnia.com
  spf: true
hosts:
- cert_expires: Oct 12 16:26:08 2026 GMT
  host: newtqnia.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 16:26:08 2026 GMT
  host: api.newtqnia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newtqnia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewTqnia | Technology News, AI and Innovation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NewTqnia | Technology News, AI and Innovation
provider_slug: newtqnia
slug: newtqnia-domain-security
source_filename: newtqnia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newtqnia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:26:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.newtqnia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:26:08 2026 GMT\n  hsts: null\ndomains:\n- domain: newtqnia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newtqnia/refs/heads/main/security/newtqnia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- News API
- News
- Technology
- Artificial Intelligence
- Cybersecurity
- Developer Tools
- Cloud Computing
- Media
- Publishing
- Bilingual
---
