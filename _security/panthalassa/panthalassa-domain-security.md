---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: panthalassa.com
  spf: true
hosts:
- cert_expires: Oct 10 23:15:20 2026 GMT
  host: panthalassa.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Panthalassa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panthalassa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Panthalassa
provider_slug: panthalassa
slug: panthalassa-domain-security
source_filename: panthalassa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: panthalassa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:15:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: panthalassa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panthalassa/refs/heads/main/security/panthalassa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Renewable Energy
- Wave Energy
- Ocean
- Data Centers
- Compute
- Climate Tech
- Hardware
- Public Benefit Corporation
---
