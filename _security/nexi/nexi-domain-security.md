---
api_specs:
- filename: nexi-build-api-openapi.yml
  format: yaml
  label: Nexi Build API
  slug: nexi-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-build-api-openapi.yml
- filename: nexi-contract-api-openapi.yml
  format: yaml
  label: Nexi Contract API
  slug: nexi-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-contract-api-openapi.yml
- filename: nexi-contracts-api-openapi.yml
  format: yaml
  label: Nexi Contracts API
  slug: nexi-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-contracts-api-openapi.yml
- filename: nexi-nexi-api-api-openapi.yml
  format: yaml
  label: Nexi Nexi API
  slug: nexi-nexi-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-nexi-api-api-openapi.yml
- filename: nexi-operations-api-openapi.yml
  format: yaml
  label: Nexi Operations API
  slug: nexi-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-operations-api-openapi.yml
- filename: nexi-orders-api-openapi.yml
  format: yaml
  label: Nexi Orders API
  slug: nexi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-orders-api-openapi.yml
- filename: nexi-paybylink-api-openapi.yml
  format: yaml
  label: Nexi Paybylink API
  slug: nexi-paybylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-paybylink-api-openapi.yml
- filename: nexi-payment-methods-api-openapi.yml
  format: yaml
  label: Nexi Payment Methods API
  slug: nexi-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/openapi/nexi-payment-methods-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nexigroup.com
  spf: true
hosts:
- cert_expires: Feb  1 07:21:32 2027 GMT
  host: www.nexigroup.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nexi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nexi
provider_slug: nexi
slug: nexi-domain-security
source_filename: nexi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexigroup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 07:21:32 2027 GMT\n  hsts: false\ndomains:\n- domain: nexigroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexi/refs/heads/main/security/nexi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Payments
- Fintech
- Europe
---
