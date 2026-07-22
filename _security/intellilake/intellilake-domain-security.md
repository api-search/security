---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intellilake.com
  spf: true
hosts:
- cert_expires: Oct 16 21:22:20 2026 GMT
  host: intellilake.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intellilake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intellilake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intellilake
provider_slug: intellilake
slug: intellilake-domain-security
source_filename: intellilake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intellilake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 21:22:20 2026 GMT\n  hsts: false\ndomains:\n- domain: intellilake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intellilake/refs/heads/main/security/intellilake-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Startup
- Venture Backed
- Anthemis
- Portfolio
---
