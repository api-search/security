---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clutch.ca
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.clutch.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clutch Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clutch Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clutch Canada
provider_slug: clutch-canada
slug: clutch-canada-domain-security
source_filename: clutch-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clutch.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: clutch.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clutch-canada/refs/heads/main/security/clutch-canada-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- E-Commerce
- Used Cars
- Auto Financing
- Retail
- Canada
- Consumer
---
