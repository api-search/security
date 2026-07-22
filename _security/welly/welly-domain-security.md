---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getwelly.com
  spf: true
hosts:
- cert_expires: Aug 28 08:19:02 2026 GMT
  host: getwelly.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Welly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Welly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Welly
provider_slug: welly
slug: welly-domain-security
source_filename: welly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getwelly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:19:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: getwelly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welly/refs/heads/main/security/welly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Wellness
- Consumer Packaged Goods
- First Aid
- Personal Care
- Ecommerce
- B Corporation
- Retail
---
