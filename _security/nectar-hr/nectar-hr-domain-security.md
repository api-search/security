---
api_specs:
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Users API
  slug: nectar-hr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Recognition API
  slug: nectar-hr-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Custom Awards API
  slug: nectar-hr-custom-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Financial Analytics API
  slug: nectar-hr-financial-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Flows API
  slug: nectar-hr-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nectarhr.com
  spf: true
hosts:
- cert_expires: Aug 16 21:52:49 2026 GMT
  host: nectarhr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 13:12:26 2026 GMT
  host: api.nectarhr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nectar Hr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nectar, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nectar
provider_slug: nectar-hr
slug: nectar-hr-domain-security
source_filename: nectar-hr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nectarhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 21:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nectarhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:12:26 2026 GMT\n  hsts: null\ndomains:\n- domain: nectarhr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/security/nectar-hr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Employee Recognition
- Rewards
- Points
- HR
- Employee Engagement
- Culture
- People Operations
---
