---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: groundspeed.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: insurancequantified.com
  spf: true
hosts:
- cert_expires: Oct  2 16:26:56 2026 GMT
  host: groundspeed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:06:21 2026 GMT
  host: insurancequantified.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groundspeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groundspeed, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Groundspeed
provider_slug: groundspeed
slug: groundspeed-domain-security
source_filename: groundspeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groundspeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:26:56 2026 GMT\n  hsts: false\n- host: insurancequantified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:06:21 2026 GMT\n  hsts: false\ndomains:\n- domain: groundspeed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: insurancequantified.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundspeed/refs/heads/main/security/groundspeed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Insurtech
- Underwriting
- Analytics
- Commercial Insurance
- Property and Casualty
- Document Processing
- Data Extraction
- Artificial Intelligence
---
