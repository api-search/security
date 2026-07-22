---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: eneryield.com
  spf: false
hosts:
- cert_expires: Sep  6 04:57:01 2026 GMT
  host: eneryield.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eneryield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eneryield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Eneryield
provider_slug: eneryield
slug: eneryield-domain-security
source_filename: eneryield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eneryield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 04:57:01 2026 GMT\n  hsts: false\ndomains:\n- domain: eneryield.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eneryield/refs/heads/main/security/eneryield-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Energy
- Utilities
- Power Grid
- Artificial Intelligence
- Analytics
- Predictive Maintenance
- Fault Detection
---
