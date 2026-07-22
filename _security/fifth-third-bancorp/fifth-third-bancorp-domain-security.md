---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 53.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.53.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fifth Third Bancorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fifth Third Bancorp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fifth Third Bancorp
provider_slug: fifth-third-bancorp
slug: fifth-third-bancorp-domain-security
source_filename: fifth-third-bancorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.53.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 53.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/security/fifth-third-bancorp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- Commercial Banking
- Consumer Lending
- Wealth Management
- Treasury Management
- Fortune 500
---
