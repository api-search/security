---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: filigran.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: opencti.io
  spf: true
hosts:
- cert_expires: Sep 17 18:11:47 2026 GMT
  host: filigran.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 09:30:51 2026 GMT
  host: docs.opencti.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 02:58:23 2026 GMT
  host: demo.opencti.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Filigran Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filigran, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Filigran
provider_slug: filigran
slug: filigran-domain-security
source_filename: filigran-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filigran.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:11:47 2026 GMT\n  hsts: false\n- host: docs.opencti.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:30:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: demo.opencti.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 02:58:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: filigran.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: opencti.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filigran/refs/heads/main/security/filigran-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Threat Intelligence
- OpenCTI
- OpenAEV
- STIX
- GraphQL
- Breach and Attack Simulation
- Open Source
- Security
---
