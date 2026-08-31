---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: claimdi.com
  spf: true
hosts:
- cert_expires: Dec 13 09:36:02 2026 GMT
  host: claimdi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anywhere 2 Go Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anywhere 2 Go, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Anywhere 2 Go
provider_slug: anywhere-2-go
slug: anywhere-2-go-domain-security
source_filename: anywhere-2-go-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claimdi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 09:36:02 2026 GMT\n  hsts: false\ndomains:\n- domain: claimdi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anywhere-2-go/refs/heads/main/security/anywhere-2-go-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Insurance
- InsurTech
- Claims
- Automotive
- Mobile
- Thailand
---
