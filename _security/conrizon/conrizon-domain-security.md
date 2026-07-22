---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conrizon.com
  spf: true
hosts:
- cert_expires: Aug 20 02:32:07 2026 GMT
  host: conrizon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conrizon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for conrizon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: conrizon
provider_slug: conrizon
slug: conrizon-domain-security
source_filename: conrizon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conrizon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 02:32:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conrizon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conrizon/refs/heads/main/security/conrizon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise Content Management
- ECM
- Document Management
- Archiving
- Invoice Processing
- Contract Management
- Human Resources
- SAP Integration
- Microsoft 365
- Germany
- B2B Software
---
