---
api_specs:
- filename: nas-academy-openapi-original.json
  format: json
  label: Nas.com Public Discovery API
  slug: nascom-public-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nas-academy/refs/heads/main/openapi/nas-academy-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nas.com
  spf: true
hosts:
- cert_expires: Sep 11 18:21:12 2026 GMT
  host: nas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nas Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nas.com (Nas Academy), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nas.com (Nas Academy)
provider_slug: nas-academy
slug: nas-academy-domain-security
source_filename: nas-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:21:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nas-academy/refs/heads/main/security/nas-academy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- Community
- E-commerce
- AI
- Agents
- MCP
- Online Courses
- Sellers
---
