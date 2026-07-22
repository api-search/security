---
api_specs:
- filename: shoppable-cloud-openapi-original.yml
  format: yaml
  label: Shoppable Commerce API Suite
  slug: shoppable-commerce-api-suite
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoppable/refs/heads/main/openapi/shoppable-cloud-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shoppable.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: shoppable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: cloud.staging.shoppable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: cloud.shoppable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shoppable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shoppable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shoppable
provider_slug: shoppable
slug: shoppable-domain-security
source_filename: shoppable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shoppable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\n- host: cloud.staging.shoppable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\n- host: cloud.shoppable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shoppable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoppable/refs/heads/main/security/shoppable-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Checkout
- Catalog
- Payments
- Agentic Commerce
- MCP
- Embeddable Commerce
- Retail
---
