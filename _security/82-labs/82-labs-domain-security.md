---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: morelabs.com
  spf: true
hosts:
- cert_expires: Aug 28 12:59:02 2026 GMT
  host: morelabs.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 82 Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 82 Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 82 Labs
provider_slug: 82-labs
slug: 82-labs-domain-security
source_filename: 82-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:59:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: morelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/82-labs/refs/heads/main/security/82-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Wellness
- Beverages
- Supplements
- Health
- Direct-to-Consumer
- E-Commerce
---
