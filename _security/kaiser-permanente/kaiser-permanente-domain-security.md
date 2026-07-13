---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaiserpermanente.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kp.org
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.kaiserpermanente.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: kp.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kaiser Permanente Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaiser Permanente, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kaiser Permanente
provider_slug: kaiser-permanente
slug: kaiser-permanente-domain-security
source_filename: kaiser-permanente-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaiserpermanente.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kp.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kaiserpermanente.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaiser-permanente/refs/heads/main/security/kaiser-permanente-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Healthcare
- Insurance
- Health Insurance
- Hospitals
- FHIR
- Interoperability
---
