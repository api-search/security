---
api_specs:
- filename: cometeer-storefront-openapi.yml
  format: yaml
  label: Cometeer Storefront (read-only)
  slug: storefront
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometeer/refs/heads/main/openapi/cometeer-storefront-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cometeer.com
  spf: true
hosts:
- cert_expires: Sep 13 22:40:33 2026 GMT
  host: cometeer.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cometeer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cometeer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cometeer
provider_slug: cometeer
slug: cometeer-domain-security
source_filename: cometeer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cometeer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:40:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: cometeer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometeer/refs/heads/main/security/cometeer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coffee
- Food and Beverage
- E-Commerce
- Direct to Consumer
- Retail
- Subscription
- Agentic Commerce
- Shopify
- Model Context Protocol
---
