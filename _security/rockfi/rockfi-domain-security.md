---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rockfi.fr
  spf: true
hosts:
- cert_expires: Aug 22 00:39:36 2026 GMT
  host: www.rockfi.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rockfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RockFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RockFi
provider_slug: rockfi
slug: rockfi-domain-security
source_filename: rockfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rockfi.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 00:39:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rockfi.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockfi/refs/heads/main/security/rockfi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Wealth Management
- Private Banking
- Fintech
- France
---
