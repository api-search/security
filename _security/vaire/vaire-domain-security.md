---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vaire.co
  spf: false
hosts:
- cert_expires: Sep 29 13:35:40 2026 GMT
  host: vaire.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vaire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vaire Computing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Vaire Computing
provider_slug: vaire
slug: vaire-domain-security
source_filename: vaire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vaire.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:35:40 2026 GMT\n  hsts: false\ndomains:\n- domain: vaire.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaire/refs/heads/main/security/vaire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Hardware
- Reversible Computing
- Energy Efficiency
- Deep Tech
- Chips
---
