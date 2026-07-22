---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pretred.com
  spf: true
hosts:
- cert_expires: Sep  6 21:58:37 2026 GMT
  host: pretred.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pretred Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pretred, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pretred
provider_slug: pretred
slug: pretred-domain-security
source_filename: pretred-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pretred.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:58:37 2026 GMT\n  hsts: false\ndomains:\n- domain: pretred.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pretred/refs/heads/main/security/pretred-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Sustainability
- Recycling
- Infrastructure
- Manufacturing
- Circular Economy
- Traffic Safety
---
