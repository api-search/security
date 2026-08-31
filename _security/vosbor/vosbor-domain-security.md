---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vosbor.com
  spf: true
hosts:
- cert_expires: Oct 14 15:52:44 2026 GMT
  host: www.vosbor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vosbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vosbor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vosbor
provider_slug: vosbor
slug: vosbor-domain-security
source_filename: vosbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vosbor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:52:44 2026 GMT\n  hsts: false\ndomains:\n- domain: vosbor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vosbor/refs/heads/main/security/vosbor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agritech
- Commodities
- Trading
- Agriculture
- Exchange
- Marketplace
- Grain
- Oilseeds
---
