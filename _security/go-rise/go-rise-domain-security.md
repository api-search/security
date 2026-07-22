---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gorise.co
  spf: true
hosts:
- cert_expires: Sep  6 22:20:45 2026 GMT
  host: gorise.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Go Rise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go Rise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Go Rise
provider_slug: go-rise
slug: go-rise-domain-security
source_filename: go-rise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gorise.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:20:45 2026 GMT\n  hsts: false\ndomains:\n- domain: gorise.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go-rise/refs/heads/main/security/go-rise-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Banking
- Financial Services
- Remittances
- Migrant
- Insurance
- Mobile
---
