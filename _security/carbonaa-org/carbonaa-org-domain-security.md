---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carbonaa.org
  spf: false
hosts:
- cert_expires: Jan 15 02:34:59 2027 GMT
  host: carbonaa.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbonaa Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbonaa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Carbonaa
provider_slug: carbonaa-org
slug: carbonaa-org-domain-security
source_filename: carbonaa-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbonaa.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 02:34:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carbonaa.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/carbonaa-org/security/carbonaa-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Software-as-a-Service
- Climate
- Carbon Management
- Sustainability
- Environmental Data
---
