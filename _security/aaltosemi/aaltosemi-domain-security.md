---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aaltosemi.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.aaltosemi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aaltosemi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aaltosemi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aaltosemi
provider_slug: aaltosemi
slug: aaltosemi-domain-security
source_filename: aaltosemi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aaltosemi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aaltosemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaltosemi/refs/heads/main/security/aaltosemi-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Semiconductors
- Semiconductor Packaging
- IC Substrates
- Advanced Packaging
- Electronics Manufacturing
- Hardware
- FCBGA
- Nanjing
- China
---
