---
api_specs:
- filename: automat-extract-openapi.json
  format: json
  label: Automat Extract API
  slug: automat-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automat/refs/heads/main/openapi/automat-extract-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: runautomat.com
  spf: true
hosts:
- cert_expires: Oct 11 01:31:28 2026 GMT
  host: www.runautomat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 08:42:33 2026 GMT
  host: docs.runautomat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 00:45:19 2026 GMT
  host: studio.runautomat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automat, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Automat
provider_slug: automat
slug: automat-domain-security
source_filename: automat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.runautomat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 01:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.runautomat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:42:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: studio.runautomat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:45:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: runautomat.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automat/refs/heads/main/security/automat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise Saas
- Automation
- RPA
- Robotic Process Automation
- Document Extraction
- IDP
- iPaaS
- AI Agents
- Computer Use
- Document Processing
---
