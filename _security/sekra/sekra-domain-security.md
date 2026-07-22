---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sekra.com
  spf: true
hosts:
- cert_expires: Oct 16 14:15:17 2026 GMT
  host: www.sekra.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sekra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sekra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sekra
provider_slug: sekra
slug: sekra-domain-security
source_filename: sekra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sekra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:15:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sekra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sekra/refs/heads/main/security/sekra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Real Estate
- Community
- Residential
- Housing
- Property Development
---
