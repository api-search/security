---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: diligentpharma.com
  spf: true
hosts:
- cert_expires: Oct 16 11:01:51 2026 GMT
  host: www.diligentpharma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diligent Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diligent Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Diligent Pharma
provider_slug: diligent-pharma
slug: diligent-pharma-domain-security
source_filename: diligent-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diligentpharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: diligentpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent-pharma/refs/heads/main/security/diligent-pharma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Clinical Trials
- Life Sciences
- Pharmaceuticals
- Biotechnology
- Vendor Management
- Risk Management
- Quality Management
- Compliance
- GxP
- Auditing
- Software-as-a-Service
---
