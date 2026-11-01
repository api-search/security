---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aiegis.ie
  spf: false
hosts:
- cert_expires: Dec  2 06:39:43 2026 GMT
  host: aiegis.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiegis Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aiegis-ie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: aiegis-ie
provider_slug: aiegis-ie
slug: aiegis-ie-domain-security
source_filename: aiegis-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiegis.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 06:39:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aiegis.ie\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aiegis-ie/security/aiegis-ie-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Identity
- Governance
- Security
---
