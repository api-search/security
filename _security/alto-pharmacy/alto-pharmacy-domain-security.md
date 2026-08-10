---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alto.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: www.alto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alto Pharmacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alto Pharmacy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alto Pharmacy
provider_slug: alto-pharmacy
slug: alto-pharmacy-domain-security
source_filename: alto-pharmacy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alto-pharmacy/refs/heads/main/security/alto-pharmacy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmacy
- Digital Health
- Healthcare
- Prescriptions
- Specialty Pharmacy
- Fertility
- Medication Delivery
- Pharmacy Technology
- Health Plans
---
