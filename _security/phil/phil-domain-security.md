---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: phil.us
  spf: true
hosts:
- cert_expires: Mar  4 18:36:13 2027 GMT
  host: www.phil.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Phil
provider_slug: phil
slug: phil-domain-security
source_filename: phil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phil.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 18:36:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: phil.us\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phil/refs/heads/main/security/phil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Healthtech
- Pharmacy
- Direct-to-Patient
- Medication Access
- Digital Health
- Prescriptions
---
