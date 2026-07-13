---
api_specs:
- filename: taboola-backstage-campaigns-api-openapi.yml
  format: yaml
  label: Taboola Backstage Campaigns API
  slug: taboola-backstage-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-campaigns-api-openapi.yml
- filename: taboola-backstage-items-api-openapi.yml
  format: yaml
  label: Taboola Backstage Campaign Items API
  slug: taboola-backstage-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-items-api-openapi.yml
- filename: taboola-backstage-audiences-api-openapi.yml
  format: yaml
  label: Taboola Backstage Audiences API
  slug: taboola-backstage-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-audiences-api-openapi.yml
- filename: taboola-backstage-conversions-api-openapi.yml
  format: yaml
  label: Taboola Backstage Conversions API
  slug: taboola-backstage-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-conversions-api-openapi.yml
- filename: taboola-backstage-reports-api-openapi.yml
  format: yaml
  label: Taboola Backstage Reports API
  slug: taboola-backstage-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-reports-api-openapi.yml
- filename: taboola-backstage-dictionary-api-openapi.yml
  format: yaml
  label: Taboola Backstage Dictionary API
  slug: taboola-backstage-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-dictionary-api-openapi.yml
- filename: taboola-backstage-accounts-api-openapi.yml
  format: yaml
  label: Taboola Backstage Accounts API
  slug: taboola-backstage-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-backstage-accounts-api-openapi.yml
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
