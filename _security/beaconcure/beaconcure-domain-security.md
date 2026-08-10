---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beaconcure.com
  spf: true
hosts:
- cert_expires: Oct 27 09:50:45 2026 GMT
  host: beaconcure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beaconcure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beaconcure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beaconcure
provider_slug: beaconcure
slug: beaconcure-domain-security
source_filename: beaconcure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beaconcure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 09:50:45 2026 GMT\n  hsts: false\ndomains:\n- domain: beaconcure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconcure/refs/heads/main/security/beaconcure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Clinical Trials
- Clinical Data
- Life Sciences
- Pharmaceuticals
- Data Validation
- Quality Control
- Artificial Intelligence
- Biometrics
- Healthcare
---
