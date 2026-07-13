---
api_specs:
- filename: openapi.yml
  format: yaml
  label: PriceMetrics Pricing API
  slug: pricemetrics-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricemetrics/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pricimetrics.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pricemetrics.com
  spf: false
hosts:
- cert_expires: Sep 12 19:36:59 2026 GMT
  host: www.pricimetrics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.pricemetrics.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pricemetrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PriceMetrics, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PriceMetrics
provider_slug: pricemetrics
slug: pricemetrics-domain-security
source_filename: pricemetrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pricimetrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:36:59 2026 GMT\n  hsts: false\n- host: api.pricemetrics.com\n  https: false\ndomains:\n- domain: pricimetrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pricemetrics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pricemetrics/refs/heads/main/security/pricemetrics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pricing
- Price Optimization
- Competitive Intelligence
- Revenue Management
- Analytics
- Elasticity Analysis
- Retail
- Commerce
---
