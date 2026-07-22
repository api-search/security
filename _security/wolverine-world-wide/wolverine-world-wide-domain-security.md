---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wolverineworldwide.com
  spf: true
hosts:
- cert_expires: Sep 30 22:12:57 2026 GMT
  host: www.wolverineworldwide.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wolverine World Wide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wolverine World Wide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wolverine World Wide
provider_slug: wolverine-world-wide
slug: wolverine-world-wide-domain-security
source_filename: wolverine-world-wide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wolverineworldwide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:12:57 2026 GMT\n  hsts: false\ndomains:\n- domain: wolverineworldwide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolverine-world-wide/refs/heads/main/security/wolverine-world-wide-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Apparel
- Consumer Goods
- eCommerce
- Footwear
- Retail
- Fortune 1000
---
