---
api_specs:
- filename: rijksmuseum-collection-openapi.yml
  format: yaml
  label: Collection Search API
  slug: collection-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-collection-openapi.yml
- filename: rijksmuseum-collection-openapi.yml
  format: yaml
  label: Collection Details API
  slug: collection-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-collection-openapi.yml
- filename: rijksmuseum-collection-openapi.yml
  format: yaml
  label: Collection Image Tiles API
  slug: collection-image-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-collection-openapi.yml
- filename: rijksmuseum-user-sets-openapi.yml
  format: yaml
  label: Usersets API
  slug: usersets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-user-sets-openapi.yml
- filename: rijksmuseum-user-sets-openapi.yml
  format: yaml
  label: Userset Details API
  slug: userset-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/openapi/rijksmuseum-user-sets-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rijksmuseum.nl
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.rijksmuseum.nl
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: data.rijksmuseum.nl
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rijksmuseum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rijksmuseum, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rijksmuseum
provider_slug: rijksmuseum
slug: rijksmuseum-domain-security
source_filename: rijksmuseum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rijksmuseum.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: data.rijksmuseum.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: rijksmuseum.nl\n  dnssec: true\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rijksmuseum/refs/heads/main/security/rijksmuseum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Art And Design
- Museums
- Cultural Heritage
- Open Data
- Linked Data
- OAI-PMH
- IIIF
- Dutch Heritage
- Public APIs
---
