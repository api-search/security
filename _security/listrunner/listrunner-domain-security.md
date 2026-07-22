---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: listrunnerapp.com
  spf: false
hosts:
- cert_expires: Sep 24 05:42:41 2026 GMT
  host: listrunnerapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Listrunner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listrunner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Listrunner
provider_slug: listrunner
slug: listrunner-domain-security
source_filename: listrunner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listrunnerapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: listrunnerapp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listrunner/refs/heads/main/security/listrunner-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Healthcare
- Clinical Collaboration
- Care Coordination
- Patient Lists
- Clinical Handoff
- HIPAA
- Mobile
- Defunct
---
