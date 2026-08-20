---
api_specs:
- filename: windstream-holdings-agents-api-openapi.yml
  format: yaml
  label: Windstream Holdings agents API
  slug: windstream-holdings-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-agents-api-openapi.yml
- filename: windstream-holdings-auto-attendants-api-openapi.yml
  format: yaml
  label: Windstream Holdings auto-attendants API
  slug: windstream-holdings-auto-attendants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-auto-attendants-api-openapi.yml
- filename: windstream-holdings-calls-api-openapi.yml
  format: yaml
  label: Windstream Holdings calls API
  slug: windstream-holdings-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-calls-api-openapi.yml
- filename: windstream-holdings-extensions-api-openapi.yml
  format: yaml
  label: Windstream Holdings extensions API
  slug: windstream-holdings-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-extensions-api-openapi.yml
- filename: windstream-holdings-products-api-openapi.yml
  format: yaml
  label: Windstream Holdings products API
  slug: windstream-holdings-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-products-api-openapi.yml
- filename: windstream-holdings-roles-api-openapi.yml
  format: yaml
  label: Windstream Holdings roles API
  slug: windstream-holdings-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-roles-api-openapi.yml
- filename: windstream-holdings-system-api-openapi.yml
  format: yaml
  label: Windstream Holdings system API
  slug: windstream-holdings-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-system-api-openapi.yml
- filename: windstream-holdings-tenants-api-openapi.yml
  format: yaml
  label: Windstream Holdings tenants API
  slug: windstream-holdings-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-tenants-api-openapi.yml
- filename: windstream-holdings-users-api-openapi.yml
  format: yaml
  label: Windstream Holdings users API
  slug: windstream-holdings-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: windstreamenterprise.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uniti.com
  spf: true
hosts:
- cert_expires: Sep  5 13:47:21 2026 GMT
  host: www.windstreamenterprise.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 04:18:42 2026 GMT
  host: api.solutions.uniti.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: webadmin.windstreamenterprise.com
  https: false
kind: domain-security
layout: security
method: probed
name: Windstream Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Windstream Holdings, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Windstream Holdings
provider_slug: windstream-holdings
slug: windstream-holdings-domain-security
source_filename: windstream-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.windstreamenterprise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:47:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.solutions.uniti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 04:18:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: webadmin.windstreamenterprise.com\n  https: false\ndomains:\n- domain: windstreamenterprise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: uniti.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/security/windstream-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadband
- Contact Center
- Managed Service
- Network Communications
- SD-WAN
- Telecom
- UCaaS
- Unified Communications
- Fortune 500
---
