---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beconfident.app
  spf: true
hosts:
- cert_expires: Aug 31 05:12:36 2026 GMT
  host: beconfident.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beconfident Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeConfident, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BeConfident
provider_slug: beconfident
slug: beconfident-domain-security
source_filename: beconfident-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beconfident.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:12:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beconfident.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beconfident/refs/heads/main/security/beconfident-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EdTech
- Language Learning
- Artificial Intelligence
- Education
- English
---
