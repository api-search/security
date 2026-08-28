---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: resynergi.com
  spf: true
hosts:
- cert_expires: Nov  2 02:01:02 2026 GMT
  host: resynergi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resynergi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resynergi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Resynergi
provider_slug: resynergi
slug: resynergi-domain-security
source_filename: resynergi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resynergi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 02:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: resynergi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resynergi/refs/heads/main/security/resynergi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Advanced Recycling
- Plastics
- Pyrolysis
- Circular Economy
- Sustainability
- Waste Management
- Energy
- Industrial Equipment
- Climate Tech
---
