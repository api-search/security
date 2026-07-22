---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frazerconsultants.com
  spf: true
hosts:
- cert_expires: Sep  2 05:31:52 2026 GMT
  host: www.frazerconsultants.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frazerconsultants Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frazer Consultants, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Frazer Consultants
provider_slug: frazerconsultants
slug: frazerconsultants-domain-security
source_filename: frazerconsultants-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frazerconsultants.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frazerconsultants.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frazerconsultants/refs/heads/main/security/frazerconsultants-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Funeral Homes
- Death Care
- Funeral Home Software
- Tribute Technology
- Memorial Websites
- Obituaries
- Payments
- Webcasting
- Partner API
- No Public API
---
