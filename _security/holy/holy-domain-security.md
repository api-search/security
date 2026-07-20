---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: holy.com
  spf: true
hosts:
- cert_expires: Oct 12 08:10:06 2026 GMT
  host: de.holy.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HOLY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HOLY
provider_slug: holy
slug: holy-domain-security
source_filename: holy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: de.holy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 08:10:06 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: holy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holy/refs/heads/main/security/holy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Beverages
- Direct-to-Consumer
- Ecommerce
- Agentic Commerce
- Shopify
- Germany
---
