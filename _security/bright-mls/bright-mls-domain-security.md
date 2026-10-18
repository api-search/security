---
api_specs:
- filename: bright-mls-auth-api-openapi.yml
  format: yaml
  label: Bright MLS Auth API
  slug: bright-mls-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-auth-api-openapi.yml
- filename: bright-mls-listing-api-openapi.yml
  format: yaml
  label: Bright MLS Listing API
  slug: bright-mls-listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-listing-api-openapi.yml
- filename: bright-mls-manifests-api-openapi.yml
  format: yaml
  label: Bright MLS Manifests API
  slug: bright-mls-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-manifests-api-openapi.yml
- filename: bright-mls-user-api-openapi.yml
  format: yaml
  label: Bright MLS User API
  slug: bright-mls-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-user-api-openapi.yml
- filename: bright-mls-data-hub-api-openapi.yml
  format: yaml
  label: Bright MLS Data Hub API
  slug: bright-mls-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-data-hub-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brightmls.com
  spf: true
hosts:
- cert_expires: Apr  7 23:59:59 2027 GMT
  host: www.brightmls.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bright Mls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright MLS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bright MLS
provider_slug: bright-mls
slug: bright-mls-domain-security
source_filename: bright-mls-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightmls.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: brightmls.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/security/bright-mls-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- MLS
- RESO
- OData
- Listings
- Property Data
---
