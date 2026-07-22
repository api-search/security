---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: byheart.com
  spf: true
hosts:
- cert_expires: Sep  7 16:33:02 2026 GMT
  host: www.byheart.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Byheart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ByHeart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ByHeart
provider_slug: byheart
slug: byheart-domain-security
source_filename: byheart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.byheart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 16:33:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: byheart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byheart/refs/heads/main/security/byheart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Infant Nutrition
- Baby Formula
- Direct-to-Consumer
- Ecommerce
- Health
- Shopify
---
