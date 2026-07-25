---
api_specs:
- filename: unmade-design-api-api-openapi.yml
  format: yaml
  label: Unmade Design API API
  slug: unmade-design-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-design-api-api-openapi.yml
- filename: unmade-ecommerce-orders-api-api-openapi.yml
  format: yaml
  label: Unmade Ecommerce Orders API API
  slug: unmade-ecommerce-orders-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-ecommerce-orders-api-api-openapi.yml
- filename: unmade-factory-api-api-openapi.yml
  format: yaml
  label: Unmade Factory API API
  slug: unmade-factory-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-factory-api-api-openapi.yml
- filename: unmade-outfit-api-api-openapi.yml
  format: yaml
  label: Unmade Outfit API API
  slug: unmade-outfit-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-outfit-api-api-openapi.yml
- filename: unmade-transfer-preview-api-api-openapi.yml
  format: yaml
  label: Unmade Transfer Preview API API
  slug: unmade-transfer-preview-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-transfer-preview-api-api-openapi.yml
- filename: unmade-unmade-editor-api-openapi.yml
  format: yaml
  label: Unmade Unmade Editor API
  slug: unmade-unmade-editor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-unmade-editor-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unmade.com
  spf: true
hosts:
- cert_expires: Sep 10 07:26:00 2026 GMT
  host: unmade.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: partner-subdomain.embed.unmade.com
  https: false
kind: domain-security
layout: security
method: probed
name: Unmade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unmade, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unmade
provider_slug: unmade
slug: unmade-domain-security
source_filename: unmade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unmade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:26:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-subdomain.embed.unmade.com\n  https: false\ndomains:\n- domain: unmade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/security/unmade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fashion
- Apparel
- Manufacturing
- Customization
- eCommerce
- On-Demand Production
- Embedded Commerce
---
