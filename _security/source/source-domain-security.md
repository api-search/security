---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: source.co
  spf: true
hosts:
- cert_expires: Sep 12 02:31:02 2026 GMT
  host: source.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Source Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SOURCE Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SOURCE Global
provider_slug: source
slug: source-domain-security
source_filename: source-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: source.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:31:02 2026 GMT\n  hsts: null\ndomains:\n- domain: source.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/source/refs/heads/main/security/source-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Water
- Drinking Water
- Cleantech
- Climate Tech
- Atmospheric Water Generation
- Hardware
- Consumer Products
- Renewable Energy
- Public Benefit Corporation
---
