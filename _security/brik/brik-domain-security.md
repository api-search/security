---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brik.id
  spf: false
hosts:
- cert_expires: Sep 20 06:56:59 2026 GMT
  host: brik.id
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Brik
provider_slug: brik
slug: brik-domain-security
source_filename: brik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brik.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:56:59 2026 GMT\n  hsts: false\ndomains:\n- domain: brik.id\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brik/refs/heads/main/security/brik-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- B2B
- Construction
- Concrete
- Ready-Mix Concrete
- Building Materials
- Indonesia
---
