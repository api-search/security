---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agromatch.cl
  spf: true
hosts:
- cert_expires: Aug 29 19:07:08 2026 GMT
  host: agromatch.cl
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agromatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgroMatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgroMatch
provider_slug: agromatch
slug: agromatch-domain-security
source_filename: agromatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agromatch.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 19:07:08 2026 GMT\n  hsts: false\ndomains:\n- domain: agromatch.cl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agromatch/refs/heads/main/security/agromatch-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AgTech
- Agriculture
- Marketplace
- Machinery Rental
- Agricultural Services
- IoT
- Chile
---
