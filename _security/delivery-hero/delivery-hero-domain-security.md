---
api_specs:
- filename: delivery-hero-on-demand-rider-openapi.json
  format: json
  label: Delivery Hero On Demand Rider API
  slug: delivery-hero-on-demand-rider
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delivery-hero/refs/heads/main/openapi/delivery-hero-on-demand-rider-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deliveryhero.com
  spf: true
hosts:
- cert_expires: Aug 29 04:37:15 2026 GMT
  host: deliveryhero.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Delivery Hero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delivery Hero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Delivery Hero
provider_slug: delivery-hero
slug: delivery-hero-domain-security
source_filename: delivery-hero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deliveryhero.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 04:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deliveryhero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delivery-hero/refs/heads/main/security/delivery-hero-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Technology
- Food Delivery
- Logistics
- Quick Commerce
- Last Mile Delivery
- On Demand
- Orders
---
