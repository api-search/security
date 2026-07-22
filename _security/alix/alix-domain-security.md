---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: meetalix.com
  spf: true
hosts:
- cert_expires: Aug 25 00:16:10 2026 GMT
  host: meetalix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Alix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Alix
provider_slug: alix
slug: alix-domain-security
source_filename: alix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meetalix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 00:16:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meetalix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alix/refs/heads/main/security/alix-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fintech
- Estate Settlement
- Legal Tech
- Probate
- Estate Administration
- Wealth
- Consumer Finance
---
