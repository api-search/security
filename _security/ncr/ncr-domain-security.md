---
api_specs:
- filename: ncr-catalog-api-openapi.yml
  format: yaml
  label: NCR Catalog API
  slug: ncr-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-catalog-api-openapi.yml
- filename: ncr-category-api-openapi.yml
  format: yaml
  label: NCR Category API
  slug: ncr-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-category-api-openapi.yml
- filename: ncr-order-api-openapi.yml
  format: yaml
  label: NCR Order API
  slug: ncr-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-order-api-openapi.yml
- filename: ncr-provisioning-api-openapi.yml
  format: yaml
  label: NCR Provisioning API
  slug: ncr-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-provisioning-api-openapi.yml
- filename: ncr-security-api-openapi.yml
  format: yaml
  label: NCR Security API
  slug: ncr-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-security-api-openapi.yml
- filename: ncr-selling-api-openapi.yml
  format: yaml
  label: NCR Selling API
  slug: ncr-selling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-selling-api-openapi.yml
- filename: ncr-site-api-openapi.yml
  format: yaml
  label: NCR Site API
  slug: ncr-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-site-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncr.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncrvoyix.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.ncr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.ncrvoyix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 09:47:56 2026 GMT
  host: www.ncratleos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ncr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NCR, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NCR
provider_slug: ncr
slug: ncr-domain-security
source_filename: ncr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ncrvoyix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ncratleos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:47:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ncr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ncrvoyix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/security/ncr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Retail
- Banking
- ATM
- Point-of-Sale
- Commerce
- Fortune 500
---
