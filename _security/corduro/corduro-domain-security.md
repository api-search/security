---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corduro.com
  spf: true
hosts:
- cert_expires: Oct  4 22:02:39 2026 GMT
  host: www.corduro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corduro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corduro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Corduro
provider_slug: corduro
slug: corduro-domain-security
source_filename: corduro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corduro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:02:39 2026 GMT\n  hsts: false\ndomains:\n- domain: corduro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corduro/refs/heads/main/security/corduro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Payments
- Fintech
- Payment Gateway
- Payment Processing
- Mobile Payments
- eCommerce
- PCI Compliance
---
