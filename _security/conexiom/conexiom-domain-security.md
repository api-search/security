---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conexiom.com
  spf: true
hosts:
- cert_expires: Aug 24 09:04:19 2026 GMT
  host: www.conexiom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conexiom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conexiom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conexiom
provider_slug: conexiom
slug: conexiom-domain-security
source_filename: conexiom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conexiom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conexiom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conexiom/refs/heads/main/security/conexiom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Software
- Order Automation
- Invoice Automation
- Document Processing
- Supply Chain
- ERP Integration
- Manufacturing
- Distribution
---
