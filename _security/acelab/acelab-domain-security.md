---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acelabusa.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: run.app
  spf: true
hosts:
- cert_expires: Oct 25 13:25:53 2026 GMT
  host: www.acelabusa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:37:15 2026 GMT
  host: acelab-api-prod-178528813198.us-east4.run.app
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 03:34:00 2026 GMT
  host: docs.acelabusa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Acelab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acelab, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acelab
provider_slug: acelab
slug: acelab-domain-security
source_filename: acelab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acelabusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:25:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: acelab-api-prod-178528813198.us-east4.run.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:37:15 2026 GMT\n  hsts: null\n- host: docs.acelabusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 03:34:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: acelabusa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: run.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acelab/refs/heads/main/security/acelab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Architecture
- Building Materials
- Design
- Sustainability
- Product Data
- AECO
- Revit
- Specification
---
