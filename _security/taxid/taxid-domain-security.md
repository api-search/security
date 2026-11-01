---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: taxid.pro
  spf: false
hosts:
- cert_expires: Nov 28 16:28:54 2026 GMT
  host: taxid.pro
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taxid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tax ID Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tax ID Pro
provider_slug: taxid
slug: taxid-domain-security
source_filename: taxid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taxid.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:28:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: taxid.pro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/taxid/security/taxid-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Tax
- Validation
- API
- Fintech
---
