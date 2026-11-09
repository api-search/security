---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: careplankit.com
  spf: true
hosts:
- cert_expires: Jan 28 09:27:34 2027 GMT
  host: careplankit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Careplankit Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarePlanKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CarePlanKit
provider_slug: careplankit-com
slug: careplankit-com-domain-security
source_filename: careplankit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careplankit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 09:27:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: careplankit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/careplankit-com/security/careplankit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Nursing
- Education
- Care Plans
- Free
- Builder
---
