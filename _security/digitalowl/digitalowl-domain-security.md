---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digitalowl.com
  spf: true
hosts:
- cert_expires: Sep 29 15:40:58 2026 GMT
  host: www.digitalowl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digitalowl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigitalOwl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DigitalOwl
provider_slug: digitalowl
slug: digitalowl-domain-security
source_filename: digitalowl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digitalowl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:40:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: digitalowl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitalowl/refs/heads/main/security/digitalowl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Insurance
- Insurtech
- Medical Records
- Underwriting
- Claims
- Legal Tech
- Artificial Intelligence
- Data API
---
