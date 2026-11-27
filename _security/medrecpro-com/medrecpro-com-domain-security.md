---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medrecpro.com
  spf: true
hosts:
- cert_expires: Jan 15 01:34:12 2027 GMT
  host: medrecpro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MedRecPro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedRecPro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MedRecPro
provider_slug: medrecpro-com
slug: medrecpro-com-domain-security
source_filename: medrecpro-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medrecpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 01:34:12 2027 GMT\n  hsts: null\ndomains:\n- domain: medrecpro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/medrecpro-com/security/medrecpro-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Healthcare
- Pharmaceuticals
- Data Management
- Open Source
---
