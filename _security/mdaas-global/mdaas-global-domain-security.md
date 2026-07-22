---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mdaas.io
  spf: false
hosts:
- cert_expires: Oct 14 16:40:35 2026 GMT
  host: mdaas.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mdaas Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MDaaS Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: MDaaS Global
provider_slug: mdaas-global
slug: mdaas-global-domain-security
source_filename: mdaas-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mdaas.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:40:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mdaas.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mdaas-global/refs/heads/main/security/mdaas-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Healthcare
- Diagnostics
- Medical Imaging
- Africa
- Health Tech
- Nigeria
- Public Health
---
