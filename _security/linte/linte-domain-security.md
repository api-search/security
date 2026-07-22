---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linte.com
  spf: true
hosts:
- cert_expires: Oct 17 21:18:38 2026 GMT
  host: linte.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Linte
provider_slug: linte
slug: linte-domain-security
source_filename: linte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:18:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linte.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linte/refs/heads/main/security/linte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contract Lifecycle Management
- Legal Tech
- Document Automation
- Artificial Intelligence
- Contract Management
- Legal Operations
- Electronic Signature
- Business Intelligence
- Brazil
- SaaS
---
