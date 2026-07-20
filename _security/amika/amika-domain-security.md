---
api_specs:
- filename: amika-openapi.json
  format: json
  label: Amika API
  slug: amika-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amika.dev
  spf: true
hosts:
- cert_expires: Sep 19 10:14:27 2026 GMT
  host: www.amika.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:04:45 2026 GMT
  host: docs.amika.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 05:01:21 2026 GMT
  host: app.amika.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amika Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amika, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amika
provider_slug: amika
slug: amika-domain-security
source_filename: amika-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amika.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 10:14:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.amika.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:04:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.amika.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:01:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amika.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/security/amika-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Coding Agents
- Developer Tools
- Sandboxes
- Infrastructure
- CI/CD
- Automation
- Software Factory
- API
---
