---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hemster.co
  spf: true
hosts:
- cert_expires: Oct 14 07:37:33 2026 GMT
  host: hemster.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hemster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hemster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hemster
provider_slug: hemster
slug: hemster-domain-security
source_filename: hemster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hemster.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:37:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hemster.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hemster/refs/heads/main/security/hemster-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fashion Technology
- Retail
- E-Commerce
- Tailoring
- Apparel
- Sustainability
- Fit
---
