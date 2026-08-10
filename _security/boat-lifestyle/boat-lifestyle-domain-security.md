---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boat-lifestyle.com
  spf: true
hosts:
- cert_expires: Oct 24 17:10:33 2026 GMT
  host: www.boat-lifestyle.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boat Lifestyle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boat Lifestyle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boat Lifestyle
provider_slug: boat-lifestyle
slug: boat-lifestyle-domain-security
source_filename: boat-lifestyle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boat-lifestyle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 17:10:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: boat-lifestyle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boat-lifestyle/refs/heads/main/security/boat-lifestyle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Electronics
- Ecommerce
- Retail
- Audio
- Wearables
- Agent Commerce
- MCP
- Shopify
- India
---
