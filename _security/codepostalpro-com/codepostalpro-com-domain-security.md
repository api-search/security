---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codepostalpro.com
  spf: false
hosts:
- cert_expires: Jan 17 07:10:37 2027 GMT
  host: codepostalpro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:39:20 2027 GMT
  host: api.codepostalpro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: CodePostalPro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodePostalPro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: CodePostalPro
provider_slug: codepostalpro-com
slug: codepostalpro-com-domain-security
source_filename: codepostalpro-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codepostalpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 07:10:37 2027 GMT\n  hsts: false\n- host: api.codepostalpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:39:20 2027 GMT\n  hsts: null\ndomains:\n- domain: codepostalpro.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/codepostalpro-com/security/codepostalpro-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Postal Codes
- ZIP Codes
- Geocoding
- Geographic Data
- Open Data
- MCP
---
