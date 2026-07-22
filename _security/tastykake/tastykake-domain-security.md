---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tastykake.com
  spf: true
hosts:
- cert_expires: Aug 27 11:02:22 2026 GMT
  host: tastykake.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tastykake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tastykake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tastykake
provider_slug: tastykake
slug: tastykake-domain-security
source_filename: tastykake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tastykake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 11:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: tastykake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tastykake/refs/heads/main/security/tastykake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bakery
- Baked Snacks
- Consumer Packaged Goods
- Food
- Snacks
---
