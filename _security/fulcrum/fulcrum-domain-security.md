---
api_specs:
- filename: fulcrum-audio-api-openapi.yml
  format: yaml
  label: Fulcrum Audio API
  slug: fulcrum-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-audio-api-openapi.yml
- filename: fulcrum-changesets-api-openapi.yml
  format: yaml
  label: Fulcrum Changesets API
  slug: fulcrum-changesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-changesets-api-openapi.yml
- filename: fulcrum-choice-lists-api-openapi.yml
  format: yaml
  label: Fulcrum Choice Lists API
  slug: fulcrum-choice-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-choice-lists-api-openapi.yml
- filename: fulcrum-classification-sets-api-openapi.yml
  format: yaml
  label: Fulcrum Classification Sets API
  slug: fulcrum-classification-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-classification-sets-api-openapi.yml
- filename: fulcrum-forms-api-openapi.yml
  format: yaml
  label: Fulcrum Forms API
  slug: fulcrum-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-forms-api-openapi.yml
- filename: fulcrum-layers-api-openapi.yml
  format: yaml
  label: Fulcrum Layers API
  slug: fulcrum-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-layers-api-openapi.yml
- filename: fulcrum-memberships-api-openapi.yml
  format: yaml
  label: Fulcrum Memberships API
  slug: fulcrum-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-memberships-api-openapi.yml
- filename: fulcrum-photos-api-openapi.yml
  format: yaml
  label: Fulcrum Photos API
  slug: fulcrum-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-photos-api-openapi.yml
- filename: fulcrum-projects-api-openapi.yml
  format: yaml
  label: Fulcrum Projects API
  slug: fulcrum-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-projects-api-openapi.yml
- filename: fulcrum-query-api-openapi.yml
  format: yaml
  label: Fulcrum Query API
  slug: fulcrum-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-query-api-openapi.yml
- filename: fulcrum-records-api-openapi.yml
  format: yaml
  label: Fulcrum Records API
  slug: fulcrum-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-records-api-openapi.yml
- filename: fulcrum-roles-api-openapi.yml
  format: yaml
  label: Fulcrum Roles API
  slug: fulcrum-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-roles-api-openapi.yml
- filename: fulcrum-signatures-api-openapi.yml
  format: yaml
  label: Fulcrum Signatures API
  slug: fulcrum-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-signatures-api-openapi.yml
- filename: fulcrum-videos-api-openapi.yml
  format: yaml
  label: Fulcrum Videos API
  slug: fulcrum-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-videos-api-openapi.yml
- filename: fulcrum-webhooks-api-openapi.yml
  format: yaml
  label: Fulcrum Webhooks API
  slug: fulcrum-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fulcrumapp.com
  spf: true
hosts:
- cert_expires: Sep  7 00:01:38 2026 GMT
  host: www.fulcrumapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 13:56:42 2026 GMT
  host: docs.fulcrumapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.fulcrumapp.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fulcrum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fulcrum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fulcrum
provider_slug: fulcrum
slug: fulcrum-domain-security
source_filename: fulcrum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fulcrumapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:01:38 2026 GMT\n  hsts: false\n- host: docs.fulcrumapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fulcrumapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: fulcrumapp.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/security/fulcrum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Collection
- Field Data
- Geospatial
- Process Management
- Mobile
---
