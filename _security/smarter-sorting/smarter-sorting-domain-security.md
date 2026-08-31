---
api_specs:
- filename: smarter-sorting-api-api-openapi.yml
  format: yaml
  label: Smarter Sorting Api(.*) API
  slug: smarter-sorting-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-api-api-openapi.yml
- filename: smarter-sorting-assets-api-openapi.yml
  format: yaml
  label: Smarter Sorting Assets(.*) API
  slug: smarter-sorting-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-assets-api-openapi.yml
- filename: smarter-sorting-docs-api-openapi.yml
  format: yaml
  label: Smarter Sorting Docs(.*) API
  slug: smarter-sorting-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-docs-api-openapi.yml
- filename: smarter-sorting-products-api-openapi.yml
  format: yaml
  label: Smarter Sorting Products API
  slug: smarter-sorting-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-products-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: smartersorting.com
  spf: true
hosts:
- cert_expires: Oct 26 02:04:20 2026 GMT
  host: www.smartersorting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:15:19 2026 GMT
  host: api.smartersorting.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smarter Sorting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smarter Sorting, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Smarter Sorting
provider_slug: smarter-sorting
slug: smarter-sorting-domain-security
source_filename: smarter-sorting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartersorting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 02:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smartersorting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:15:19 2026 GMT\n  hsts: null\ndomains:\n- domain: smartersorting.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/security/smarter-sorting-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Product Data
- Regulatory Compliance
- Hazardous Waste
- Retail
- Consumer Goods
- Supply Chain
- Sustainability
- Dangerous Goods
- Product Classification
---
