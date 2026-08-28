---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qnovia.com
  spf: false
hosts:
- cert_expires: Sep 21 08:17:02 2026 GMT
  host: qnovia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qnovia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qnovia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Qnovia
provider_slug: qnovia
slug: qnovia-domain-security
source_filename: qnovia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qnovia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:17:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qnovia.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qnovia/refs/heads/main/security/qnovia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Pharmaceuticals
- Medical Devices
- Drug Delivery
- Digital Health
- Digital Therapeutics
- Respiratory
- Smoking Cessation
- Connected Devices
- Clinical Trials
- Artificial Intelligence
- Health
---
