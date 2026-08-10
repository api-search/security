---
api_specs:
- filename: redefine-meat-wc-store-v1-api-openapi.yml
  format: yaml
  label: Redefine Meat Wc/store/v1 API
  slug: redefine-meat-wc-store-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/openapi/redefine-meat-wc-store-v1-api-openapi.yml
- filename: redefine-meat-wp-v2-api-openapi.yml
  format: yaml
  label: Redefine Meat Wp/v2 API
  slug: redefine-meat-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/openapi/redefine-meat-wp-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: redefinemeat.com
  spf: true
hosts:
- cert_expires: Oct 17 11:31:15 2026 GMT
  host: www.redefinemeat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redefine Meat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redefine Meat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Redefine Meat
provider_slug: redefine-meat
slug: redefine-meat-domain-security
source_filename: redefine-meat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redefinemeat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:31:15 2026 GMT\n  hsts: false\ndomains:\n- domain: redefinemeat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/security/redefine-meat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Food and Beverage
- Alternative Protein
- Plant-Based
- Food Technology
- Manufacturing
- E-Commerce
- WooCommerce
- WordPress
- Retail
- Model Context Protocol
---
