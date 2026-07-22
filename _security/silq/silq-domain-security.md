---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onesilq.com
  spf: true
hosts:
- cert_expires: Sep 13 04:36:27 2026 GMT
  host: www.onesilq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Silq
provider_slug: silq
slug: silq-domain-security
source_filename: silq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onesilq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:36:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onesilq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silq/refs/heads/main/security/silq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freight Forwarding
- Logistics
- Supply Chain
- Shipping
- Customs Brokerage
- Ocean Freight
- Air Freight
---
