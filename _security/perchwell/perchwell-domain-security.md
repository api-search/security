---
api_specs:
- filename: perchwell-listings-api-openapi.yml
  format: yaml
  label: Perchwell Listings API
  slug: perchwell-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-listings-api-openapi.yml
- filename: perchwell-media-api-openapi.yml
  format: yaml
  label: Perchwell Media API
  slug: perchwell-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-media-api-openapi.yml
- filename: perchwell-member-api-openapi.yml
  format: yaml
  label: Perchwell Member API
  slug: perchwell-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-member-api-openapi.yml
- filename: perchwell-metadata-api-openapi.yml
  format: yaml
  label: Perchwell Metadata API
  slug: perchwell-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-metadata-api-openapi.yml
- filename: perchwell-office-api-openapi.yml
  format: yaml
  label: Perchwell Office API
  slug: perchwell-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-office-api-openapi.yml
- filename: perchwell-openhouse-api-openapi.yml
  format: yaml
  label: Perchwell OpenHouse API
  slug: perchwell-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-openhouse-api-openapi.yml
- filename: perchwell-property-api-openapi.yml
  format: yaml
  label: Perchwell Property API
  slug: perchwell-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-property-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: perchwell.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: perchwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: docs.perchwell.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.perchwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Perchwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perchwell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Perchwell
provider_slug: perchwell
slug: perchwell-domain-security
source_filename: perchwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perchwell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.perchwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: www.perchwell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: perchwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/security/perchwell-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Real-Estate
- MLS
- Listings
- Property Data
- RESO
- RETS
- OData
- Real Estate Data
---
