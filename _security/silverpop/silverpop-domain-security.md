---
api_specs:
- filename: silverpop-authentication-api-openapi.yml
  format: yaml
  label: Silverpop Authentication API
  slug: silverpop-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-authentication-api-openapi.yml
- filename: silverpop-campaigns-api-openapi.yml
  format: yaml
  label: Silverpop Campaigns API
  slug: silverpop-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-campaigns-api-openapi.yml
- filename: silverpop-contacts-api-openapi.yml
  format: yaml
  label: Silverpop Contacts API
  slug: silverpop-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-contacts-api-openapi.yml
- filename: silverpop-programs-api-openapi.yml
  format: yaml
  label: Silverpop Programs API
  slug: silverpop-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-programs-api-openapi.yml
- filename: silverpop-reports-api-openapi.yml
  format: yaml
  label: Silverpop Reports API
  slug: silverpop-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-reports-api-openapi.yml
- filename: silverpop-transactional-api-openapi.yml
  format: yaml
  label: Silverpop Transactional API
  slug: silverpop-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-transactional-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goacoustic.com
  spf: true
hosts:
- cert_expires: Oct  2 20:13:42 2026 GMT
  host: developer.goacoustic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api-campaign-us-1.goacoustic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api-campaign-eu-1.goacoustic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silverpop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silverpop, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Silverpop
provider_slug: silverpop
slug: silverpop-domain-security
source_filename: silverpop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.goacoustic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-campaign-us-1.goacoustic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\n- host: api-campaign-eu-1.goacoustic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goacoustic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/security/silverpop-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Email Marketing
- Marketing Automation
- Campaign Management
- Digital Marketing
---
