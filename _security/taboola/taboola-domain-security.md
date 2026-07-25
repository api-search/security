---
api_specs:
- filename: taboola-accounts-api-openapi.yml
  format: yaml
  label: Taboola Accounts API
  slug: taboola-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-accounts-api-openapi.yml
- filename: taboola-audience-targeting-api-openapi.yml
  format: yaml
  label: Taboola Audience Targeting API
  slug: taboola-audience-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-audience-targeting-api-openapi.yml
- filename: taboola-bulk-items-api-openapi.yml
  format: yaml
  label: Taboola Bulk Items API
  slug: taboola-bulk-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-items-api-openapi.yml
- filename: taboola-bulk-operations-api-openapi.yml
  format: yaml
  label: Taboola Bulk Operations API
  slug: taboola-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-operations-api-openapi.yml
- filename: taboola-campaign-items-api-openapi.yml
  format: yaml
  label: Taboola Campaign Items API
  slug: taboola-campaign-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaign-items-api-openapi.yml
- filename: taboola-campaigns-api-openapi.yml
  format: yaml
  label: Taboola Campaigns API
  slug: taboola-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaigns-api-openapi.yml
- filename: taboola-combined-audiences-api-openapi.yml
  format: yaml
  label: Taboola Combined Audiences API
  slug: taboola-combined-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-combined-audiences-api-openapi.yml
- filename: taboola-conversion-rules-api-openapi.yml
  format: yaml
  label: Taboola Conversion Rules API
  slug: taboola-conversion-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-conversion-rules-api-openapi.yml
- filename: taboola-custom-audiences-api-openapi.yml
  format: yaml
  label: Taboola Custom Audiences API
  slug: taboola-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-custom-audiences-api-openapi.yml
- filename: taboola-dictionary-api-openapi.yml
  format: yaml
  label: Taboola Dictionary API
  slug: taboola-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-dictionary-api-openapi.yml
- filename: taboola-first-party-audiences-api-openapi.yml
  format: yaml
  label: Taboola First Party Audiences API
  slug: taboola-first-party-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-first-party-audiences-api-openapi.yml
- filename: taboola-lookalike-audiences-api-openapi.yml
  format: yaml
  label: Taboola Lookalike Audiences API
  slug: taboola-lookalike-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-lookalike-audiences-api-openapi.yml
- filename: taboola-marketplace-audiences-api-openapi.yml
  format: yaml
  label: Taboola Marketplace Audiences API
  slug: taboola-marketplace-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-marketplace-audiences-api-openapi.yml
- filename: taboola-reach-estimator-api-openapi.yml
  format: yaml
  label: Taboola Reach Estimator API
  slug: taboola-reach-estimator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reach-estimator-api-openapi.yml
- filename: taboola-reports-api-openapi.yml
  format: yaml
  label: Taboola Reports API
  slug: taboola-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reports-api-openapi.yml
- filename: taboola-video-items-api-openapi.yml
  format: yaml
  label: Taboola Video Items API
  slug: taboola-video-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-video-items-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:security@taboola.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: taboola.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.taboola.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: developers.taboola.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: backstage.taboola.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taboola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taboola, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Taboola
provider_slug: taboola
slug: taboola-domain-security
source_filename: taboola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.taboola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.taboola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: backstage.taboola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taboola.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:security@taboola.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/security/taboola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Advertising
- Native Advertising
- Discovery
- Performance Marketing
- AdTech
- Realize
- Backstage
- Recommendation
- Publisher
- Programmatic
---
