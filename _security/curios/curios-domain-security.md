---
api_specs:
- filename: curios-collections-api-openapi.yml
  format: yaml
  label: Curios Collections API
  slug: curios-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/curios-collections-api-openapi.yml
- filename: curios-contracts-api-openapi.yml
  format: yaml
  label: Curios Contracts API
  slug: curios-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/curios-contracts-api-openapi.yml
- filename: curios-customers-api-openapi.yml
  format: yaml
  label: Curios Customers API
  slug: curios-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/curios-customers-api-openapi.yml
- filename: curios-listings-api-openapi.yml
  format: yaml
  label: Curios Listings API
  slug: curios-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/curios-listings-api-openapi.yml
- filename: curios-orders-api-openapi.yml
  format: yaml
  label: Curios Orders API
  slug: curios-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/curios-orders-api-openapi.yml
- filename: curios-projects-api-openapi.yml
  format: yaml
  label: Curios Projects API
  slug: curios-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/curios-projects-api-openapi.yml
- filename: curios-tokens-api-openapi.yml
  format: yaml
  label: Curios Tokens API
  slug: curios-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/curios-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: curios.com
  spf: true
hosts:
- cert_expires: Jan  6 12:16:12 2027 GMT
  host: www.curios.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Curios
provider_slug: curios
slug: curios-domain-security
source_filename: curios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:16:12 2027 GMT\n  hsts: false\ndomains:\n- domain: curios.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/security/curios-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Marketplace
- Web3
- Creators
---
