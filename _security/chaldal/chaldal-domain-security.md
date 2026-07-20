---
api_specs:
- filename: chaldal-eggtransport-openapi-original.json
  format: json
  label: Chaldal Egg Transport (Gogo Bangla) Delivery API
  slug: chaldal-egg-transport-gogo-bangla-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaldal/refs/heads/main/openapi/chaldal-eggtransport-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chaldal.com
  spf: true
hosts:
- cert_expires: Sep 25 01:32:24 2026 GMT
  host: chaldal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chaldal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chaldal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chaldal
provider_slug: chaldal
slug: chaldal-domain-security
source_filename: chaldal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaldal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:32:24 2026 GMT\n  hsts: null\ndomains:\n- domain: chaldal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaldal/refs/heads/main/security/chaldal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Grocery
- Delivery
- Logistics
- Third Party Logistics
- Ecommerce
- Supply Chain
- Bangladesh
---
