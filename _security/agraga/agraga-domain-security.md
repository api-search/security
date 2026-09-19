---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agraga.com
  spf: true
hosts:
- cert_expires: Nov 26 17:15:14 2026 GMT
  host: www.agraga.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agraga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agraga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agraga
provider_slug: agraga
slug: agraga-domain-security
source_filename: agraga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agraga.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 17:15:14 2026 GMT\n  hsts: false\ndomains:\n- domain: agraga.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agraga/refs/heads/main/security/agraga-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Freight
- Freight Forwarding
- Supply Chain
- Shipping
- Customs
- Warehousing
- Embedded Finance
- Trade
- India
- Company
---
