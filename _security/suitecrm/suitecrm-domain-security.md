---
api_specs:
- filename: suitecrm-access-token-api-openapi.yml
  format: yaml
  label: SuiteCRM Access Token API
  slug: suitecrm-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-access-token-api-openapi.yml
- filename: suitecrm-authorize-api-openapi.yml
  format: yaml
  label: SuiteCRM Authorize API
  slug: suitecrm-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-authorize-api-openapi.yml
- filename: suitecrm-current-user-api-openapi.yml
  format: yaml
  label: SuiteCRM Current User API
  slug: suitecrm-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-current-user-api-openapi.yml
- filename: suitecrm-listview-api-openapi.yml
  format: yaml
  label: SuiteCRM Listview API
  slug: suitecrm-listview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-listview-api-openapi.yml
- filename: suitecrm-logout-api-openapi.yml
  format: yaml
  label: SuiteCRM Logout API
  slug: suitecrm-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-logout-api-openapi.yml
- filename: suitecrm-meta-api-openapi.yml
  format: yaml
  label: SuiteCRM Meta API
  slug: suitecrm-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-meta-api-openapi.yml
- filename: suitecrm-module-api-openapi.yml
  format: yaml
  label: SuiteCRM Module API
  slug: suitecrm-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-module-api-openapi.yml
- filename: suitecrm-search-defs-api-openapi.yml
  format: yaml
  label: SuiteCRM Search Defs API
  slug: suitecrm-search-defs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-search-defs-api-openapi.yml
- filename: suitecrm-user-preferences-api-openapi.yml
  format: yaml
  label: SuiteCRM User Preferences API
  slug: suitecrm-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/openapi/suitecrm-user-preferences-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: suitecrm.com
  spf: true
hosts:
- cert_expires: Nov 19 17:44:49 2026 GMT
  host: suitecrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Suitecrm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuiteCRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SuiteCRM
provider_slug: suitecrm
slug: suitecrm-domain-security
source_filename: suitecrm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suitecrm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 17:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: suitecrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suitecrm/refs/heads/main/security/suitecrm-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- CRM
- Open Source
- Software-as-a-Service
- Self-Hosted
- Enterprise
---
