---
api_specs:
- filename: smarty-lookup-api-openapi.yml
  format: yaml
  label: Smarty Lookup API
  slug: smarty-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-lookup-api-openapi.yml
- filename: smarty-reverse-geo-api-openapi.yml
  format: yaml
  label: Smarty reverse-geo API
  slug: smarty-reverse-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-reverse-geo-api-openapi.yml
- filename: smarty-street-address-api-openapi.yml
  format: yaml
  label: Smarty street-address API
  slug: smarty-street-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-street-address-api-openapi.yml
- filename: smarty-us-enrichment-api-openapi.yml
  format: yaml
  label: Smarty us-enrichment API
  slug: smarty-us-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-enrichment-api-openapi.yml
- filename: smarty-us-extract-api-api-openapi.yml
  format: yaml
  label: Smarty US Extract API API
  slug: smarty-us-extract-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-extract-api-api-openapi.yml
- filename: smarty-verify-api-openapi.yml
  format: yaml
  label: Smarty Verify API
  slug: smarty-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-verify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smarty.com
  spf: true
hosts:
- cert_expires: Sep 14 04:52:55 2026 GMT
  host: www.smarty.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:12:21 2026 GMT
  host: us-street.api.smarty.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:12:21 2026 GMT
  host: us-autocomplete-pro.api.smarty.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smarty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smarty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smarty
provider_slug: smarty
slug: smarty-domain-security
source_filename: smarty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smarty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:52:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us-street.api.smarty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:12:21 2026 GMT\n  hsts: null\n- host: us-autocomplete-pro.api.smarty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:12:21 2026 GMT\n  hsts: null\ndomains:\n- domain: smarty.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/security/smarty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Address Verification
- Geocoding
- Address Autocomplete
- ZIP Code
- Address Intelligence
- Location Data
- International Address
- US Address
---
