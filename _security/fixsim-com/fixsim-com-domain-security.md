---
api_specs:
- filename: fixsim-com-executionsin-api-openapi.yml
  format: yaml
  label: FIXSIM Executions In API
  slug: fixsim-com-executionsin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-executionsin-api-openapi.yml
- filename: fixsim-com-executionsout-api-openapi.yml
  format: yaml
  label: FIXSIM Executions Out API
  slug: fixsim-com-executionsout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-executionsout-api-openapi.yml
- filename: fixsim-com-instances-api-openapi.yml
  format: yaml
  label: FIXSIM Instances API
  slug: fixsim-com-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-instances-api-openapi.yml
- filename: fixsim-com-ordersin-api-openapi.yml
  format: yaml
  label: FIXSIM Orders In API
  slug: fixsim-com-ordersin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-ordersin-api-openapi.yml
- filename: fixsim-com-ordersout-api-openapi.yml
  format: yaml
  label: FIXSIM Orders Out API
  slug: fixsim-com-ordersout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-ordersout-api-openapi.yml
- filename: fixsim-com-rawmessages-api-openapi.yml
  format: yaml
  label: FIXSIM Raw Messages API
  slug: fixsim-com-rawmessages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-rawmessages-api-openapi.yml
- filename: fixsim-com-securities-api-openapi.yml
  format: yaml
  label: FIXSIM Securities API
  slug: fixsim-com-securities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-securities-api-openapi.yml
- filename: fixsim-com-sessions-api-openapi.yml
  format: yaml
  label: FIXSIM Sessions API
  slug: fixsim-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-sessions-api-openapi.yml
- filename: fixsim-com-sessionsettings-api-openapi.yml
  format: yaml
  label: FIXSIM Session Settings API
  slug: fixsim-com-sessionsettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-sessionsettings-api-openapi.yml
- filename: fixsim-com-sso-api-openapi.yml
  format: yaml
  label: FIXSIM SSO API
  slug: fixsim-com-sso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-sso-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fixsim.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: fixsim.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FIXSIM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIXSIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FIXSIM
provider_slug: fixsim-com
slug: fixsim-com-domain-security
source_filename: fixsim-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixsim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fixsim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fixsim-com/security/fixsim-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FIX
- FIX Protocol
- Testing
- Sandbox
- Financial Services
---
