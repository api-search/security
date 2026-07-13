---
api_specs:
- filename: integrations
  format: yaml
  label: Stord API
  slug: stord-api
  spec_type: OpenAPI
  url: https://www.stord.com/integrations
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stord.com
  spf: true
hosts:
- cert_expires: Sep 11 07:56:27 2026 GMT
  host: www.stord.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 00:45:26 2026 GMT
  host: cloud.stord.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stord, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stord
provider_slug: stord
slug: stord-domain-security
source_filename: stord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:56:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.stord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:45:26 2026 GMT\n  hsts: false\ndomains:\n- domain: stord.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stord/refs/heads/main/security/stord-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce Fulfillment
- Order Management
- Inventory Management
- Shipment Tracking
- Returns Management
- Warehouse Management
- Logistics
- Supply Chain
- Shopify Integration
- BigCommerce Integration
- ERP Integration
- EDI
---
