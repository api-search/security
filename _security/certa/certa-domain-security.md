---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: certa.ai
  spf: true
hosts:
- cert_expires: Oct 15 11:14:10 2026 GMT
  host: www.certa.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Certa
provider_slug: certa
slug: certa-domain-security
source_filename: certa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.certa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:14:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: certa.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certa/refs/heads/main/security/certa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Third-Party Risk Management
- TPRM
- Compliance
- Procurement
- Vendor Management
- Risk Management
- ESG
- KYC
- Supplier Onboarding
---
