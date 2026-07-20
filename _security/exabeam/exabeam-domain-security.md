---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exabeam.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exabeam.cloud
  spf: true
hosts:
- cert_expires: Sep 12 16:04:24 2026 GMT
  host: exabeam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:01:45 2026 GMT
  host: developers.exabeam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 16:04:44 2026 GMT
  host: api.us-west.exabeam.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exabeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exabeam, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Exabeam
provider_slug: exabeam
slug: exabeam-domain-security
source_filename: exabeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exabeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.exabeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:01:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.us-west.exabeam.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:04:44 2026 GMT\n  hsts: null\ndomains:\n- domain: exabeam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: exabeam.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exabeam/refs/heads/main/security/exabeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Security
- SIEM
- UEBA
- Threat Detection
- Security Operations
- SOC
- Log Management
- Incident Response
---
