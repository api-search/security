---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aub.edu.lb
  spf: true
hosts:
- cert_expires: Dec  6 06:57:03 2026 GMT
  host: www.aub.edu.lb
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 08:52:56 2026 GMT
  host: scholarworks.aub.edu.lb
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 09:48:53 2027 GMT
  host: servicedesk.aub.edu.lb
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American University of Beirut, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: American University of Beirut
provider_slug: aub
slug: aub-domain-security
source_filename: aub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aub.edu.lb\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 06:57:03 2026 GMT\n  hsts: false\n- host: scholarworks.aub.edu.lb\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 08:52:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: servicedesk.aub.edu.lb\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 09:48:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aub.edu.lb\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aub/refs/heads/main/security/aub-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Lebanon
- Middle East
- Research
- Libraries
- Open Access
---
