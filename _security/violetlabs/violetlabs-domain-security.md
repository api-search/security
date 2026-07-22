---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: violetlabs.com
  spf: true
hosts:
- cert_expires: Sep 21 01:04:08 2026 GMT
  host: violetlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:17:45 2026 GMT
  host: docs.violetlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: app.violetlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Violetlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Violetlabs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Violetlabs
provider_slug: violetlabs
slug: violetlabs-domain-security
source_filename: violetlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: violetlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:04:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.violetlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:17:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.violetlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: violetlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/violetlabs/refs/heads/main/security/violetlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Engineering
- Manufacturing
- PLM
- ERP
- Data Integration
- Requirements Management
- Aerospace
- Defense
- MCP
- Systems Engineering
---
