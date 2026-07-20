---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flaviar.com
  spf: true
hosts:
- cert_expires: Sep 19 03:00:32 2026 GMT
  host: flaviar.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flaviar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flaviar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flaviar
provider_slug: flaviar
slug: flaviar-domain-security
source_filename: flaviar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flaviar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:00:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: flaviar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flaviar/refs/heads/main/security/flaviar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Spirits
- Whiskey
- Ecommerce
- Retail
- Beverages
- Subscription
- Agent Commerce
- Shopify
---
