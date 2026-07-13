---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: theshippersgroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kencogroup.com
  spf: true
hosts:
- cert_expires: Sep 17 01:49:10 2026 GMT
  host: www.theshippersgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:19:37 2026 GMT
  host: www.kencogroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shippers Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Shippers Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Shippers Group
provider_slug: shippers-group
slug: shippers-group-domain-security
source_filename: shippers-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theshippersgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:49:10 2026 GMT\n  hsts: null\n- host: www.kencogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:19:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theshippersgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kencogroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippers-group/refs/heads/main/security/shippers-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Third-Party Logistics
- Warehousing
- Fulfillment
- Supply Chain
- Transportation Management
- Co-Packaging
- Consumer Packaged Goods
---
