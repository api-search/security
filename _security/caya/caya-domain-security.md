---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: caya.com
  spf: true
hosts:
- cert_expires: Oct  1 04:59:57 2026 GMT
  host: www.caya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Caya
provider_slug: caya
slug: caya-domain-security
source_filename: caya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:59:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caya/refs/heads/main/security/caya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Document Automation
- Intelligent Document Processing
- Document Management
- OCR
- Data Extraction
- Mail Digitization
- Compliance
- Germany
---
