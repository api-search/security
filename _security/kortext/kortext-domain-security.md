---
api_specs:
- filename: kortext-labs-api-openapi.json
  format: json
  label: Kortext Labs AI Study Tools API
  slug: kortext-labs-ai-study-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-labs-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kortext.com
  spf: true
hosts:
- cert_expires: Sep 28 12:49:42 2026 GMT
  host: kortext.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 14:57:05 2026 GMT
  host: api-demo.labs.kortext.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 08:12:53 2026 GMT
  host: vle.kortext.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kortext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kortext, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kortext
provider_slug: kortext
slug: kortext-domain-security
source_filename: kortext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kortext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:49:42 2026 GMT\n  hsts: false\n- host: api-demo.labs.kortext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 14:57:05 2026 GMT\n  hsts: null\n- host: vle.kortext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 08:12:53 2026 GMT\n  hsts: false\ndomains:\n- domain: kortext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/security/kortext-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Higher Education
- Digital Textbooks
- Learning Analytics
- Artificial Intelligence
- Content Delivery
- LTI
- Libraries
- Student Engagement
- Publishing
---
