---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gentem.com
  spf: false
hosts:
- cert_expires: Aug 28 11:04:33 2026 GMT
  host: gentem.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gentem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gentem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gentem
provider_slug: gentem
slug: gentem-domain-security
source_filename: gentem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gentem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:04:33 2026 GMT\n  hsts: null\ndomains:\n- domain: gentem.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gentem/refs/heads/main/security/gentem-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Medical Billing
- Health Tech
- Fintech
- Payments
- Insurance Claims
---
