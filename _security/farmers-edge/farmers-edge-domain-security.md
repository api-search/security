---
api_specs:
- filename: farmers-edge-canplug-api-openapi.yml
  format: yaml
  label: Farmers Edge canplug API
  slug: farmers-edge-canplug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-canplug-api-openapi.yml
- filename: farmers-edge-carbon-api-openapi.yml
  format: yaml
  label: Farmers Edge carbon API
  slug: farmers-edge-carbon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-carbon-api-openapi.yml
- filename: farmers-edge-client-api-openapi.yml
  format: yaml
  label: Farmers Edge client API
  slug: farmers-edge-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-client-api-openapi.yml
- filename: farmers-edge-contact-api-openapi.yml
  format: yaml
  label: Farmers Edge contact API
  slug: farmers-edge-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-contact-api-openapi.yml
- filename: farmers-edge-gridcalc-api-openapi.yml
  format: yaml
  label: Farmers Edge gridcalc API
  slug: farmers-edge-gridcalc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-gridcalc-api-openapi.yml
- filename: farmers-edge-hefty-api-openapi.yml
  format: yaml
  label: Farmers Edge hefty API
  slug: farmers-edge-hefty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-hefty-api-openapi.yml
- filename: farmers-edge-integrations-api-openapi.yml
  format: yaml
  label: Farmers Edge integrations API
  slug: farmers-edge-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-integrations-api-openapi.yml
- filename: farmers-edge-labcommand-api-openapi.yml
  format: yaml
  label: Farmers Edge labcommand API
  slug: farmers-edge-labcommand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-labcommand-api-openapi.yml
- filename: farmers-edge-payments-api-openapi.yml
  format: yaml
  label: Farmers Edge payments API
  slug: farmers-edge-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-payments-api-openapi.yml
- filename: farmers-edge-recengine-api-openapi.yml
  format: yaml
  label: Farmers Edge recengine API
  slug: farmers-edge-recengine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-recengine-api-openapi.yml
- filename: farmers-edge-token-login-api-openapi.yml
  format: yaml
  label: Farmers Edge token-login API
  slug: farmers-edge-token-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-token-login-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: farmcommand.com
  spf: false
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.farmcommand.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: developer.farmcommand.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: admin.farmcommand.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farmers Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmers Edge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Farmers Edge
provider_slug: farmers-edge
slug: farmers-edge-domain-security
source_filename: farmers-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.farmcommand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.farmcommand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: admin.farmcommand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farmcommand.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/security/farmers-edge-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise
- Agriculture
- Precision Agriculture
- AgTech
- Farm Management
- Digital Agriculture
- IoT
- Weather
- Carbon
- API
---
