---
api_specs:
- filename: brooklinen-storefront-openapi.yml
  format: yaml
  label: Brooklinen Shopify Storefront JSON API
  slug: brooklinen-shopify-storefront-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-storefront-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brooklinen.com
  spf: true
hosts:
- cert_expires: Oct 28 05:40:01 2026 GMT
  host: www.brooklinen.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brooklinen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brooklinen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brooklinen
provider_slug: brooklinen
slug: brooklinen-domain-security
source_filename: brooklinen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brooklinen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 05:40:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: brooklinen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/security/brooklinen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ecommerce
- retail
- direct-to-consumer
- home-goods
- bedding
- shopify
- agentic-commerce
- universal-commerce-protocol
- mcp
- agent-native
- catalog
- checkout
---
