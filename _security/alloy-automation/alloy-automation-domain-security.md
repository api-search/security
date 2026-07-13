---
api_specs:
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Users API
  slug: alloy-automation-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation User Tokens API
  slug: alloy-automation-user-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Credentials API
  slug: alloy-automation-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Integrations API
  slug: alloy-automation-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Connectivity API
  slug: alloy-automation-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Passthrough API
  slug: alloy-automation-passthrough-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Events API
  slug: alloy-automation-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Unified Commerce API
  slug: alloy-automation-unified-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Unified CRM API
  slug: alloy-automation-unified-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Unified Accounting API
  slug: alloy-automation-unified-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: runalloy.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: runalloy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 19:15:53 2026 GMT
  host: docs.runalloy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: embedded.runalloy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alloy Automation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alloy Automation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alloy Automation
provider_slug: alloy-automation
slug: alloy-automation-domain-security
source_filename: alloy-automation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runalloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n- host: docs.runalloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:15:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: embedded.runalloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: runalloy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/security/alloy-automation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- iPaaS
- Integration
- Unified API
- Embedded
- SaaS
- Automation
---
