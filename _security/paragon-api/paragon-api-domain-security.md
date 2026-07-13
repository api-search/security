---
api_specs:
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon Connect API
  slug: paragon-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon Workflows API
  slug: paragon-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon ActionKit API
  slug: paragon-actionkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon Proxy API
  slug: paragon-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useparagon.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:stspg-customer.com -all
hosts:
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: www.useparagon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: Framer
  tls_issuer: ZeroSSL ECC DV SSL CA 2
- cert_expires: Oct  8 05:33:24 2026 GMT
  host: api.useparagon.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  https: true
  server: cloudflare
  tls_issuer: Google Trust Services (WE1)
- cert_expires: Oct  8 05:33:24 2026 GMT
  host: proxy.useparagon.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  https: true
  server: cloudflare
  tls_issuer: Google Trust Services (WE1)
- cert_expires: Oct  8 05:33:24 2026 GMT
  host: actionkit.useparagon.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  https: true
  server: cloudflare
  tls_issuer: Google Trust Services (WE1)
- cert_expires: Oct  8 05:33:24 2026 GMT
  host: zeus.useparagon.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  https: true
  server: cloudflare
  tls_issuer: Google Trust Services (WE1)
kind: domain-security
layout: security
method: probed
name: Paragon Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paragon, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS; 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paragon
provider_slug: paragon-api
slug: paragon-api-domain-security
source_filename: paragon-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.useparagon.com\n  https: true\n  tls_issuer: ZeroSSL ECC DV SSL CA 2\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: Framer\n- host: api.useparagon.com\n  https: true\n  tls_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  8 05:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  server: cloudflare\n- host: proxy.useparagon.com\n  https: true\n  tls_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  8 05:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  server: cloudflare\n- host: actionkit.useparagon.com\n  https: true\n  tls_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  8 05:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  server: cloudflare\n- host: zeus.useparagon.com\n\
  \  https: true\n  tls_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  8 05:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  server: cloudflare\ndomains:\n- domain: useparagon.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:stspg-customer.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/security/paragon-api-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Embedded iPaaS
- Integrations
- Embedded Integrations
- Native Integrations
- Workflow Automation
- Integration Platform
- API Integration
- SaaS Integrations
- Connectors
---
