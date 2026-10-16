---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buymed.com
  spf: true
hosts:
- cert_expires: Dec  1 12:56:42 2026 GMT
  host: www.buymed.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buymed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buymed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Buymed
provider_slug: buymed
slug: buymed-domain-security
source_filename: buymed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buymed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 12:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: buymed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buymed/refs/heads/main/security/buymed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- SupplyChain
- Vietnam
- SoutheastAsia
---
