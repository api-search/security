---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modifi.com
  spf: true
hosts:
- cert_expires: Sep 23 19:00:22 2026 GMT
  host: developer.modifi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MODIFI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MODIFI
provider_slug: modifi
slug: modifi-domain-security
source_filename: modifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.modifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:00:22 2026 GMT\n  hsts: null\ndomains:\n- domain: modifi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modifi/refs/heads/main/security/modifi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Trade Finance
- Financing
- Partnerships
- Transactions
---
