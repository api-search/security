---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getmayd.com
  spf: false
hosts:
- cert_expires: Oct 17 01:17:14 2026 GMT
  host: www.getmayd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mayd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MAYD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MAYD
provider_slug: mayd
slug: mayd-domain-security
source_filename: mayd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmayd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:17:14 2026 GMT\n  hsts: false\ndomains:\n- domain: getmayd.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mayd/refs/heads/main/security/mayd-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Pharmacy
- Medication Delivery
- On-Demand Delivery
- Digital Health
- E-Commerce
- Logistics
---
