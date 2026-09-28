---
api_specs:
- filename: automation-preflight-api-acceptance-pack-api-openapi.yml
  format: yaml
  label: Automation Preflight API Acceptance Pack API
  slug: automation-preflight-api-acceptance-pack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-acceptance-pack-api-openapi.yml
- filename: automation-preflight-api-analyze-api-openapi.yml
  format: yaml
  label: Automation Preflight API Analyze API
  slug: automation-preflight-api-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-analyze-api-openapi.yml
- filename: automation-preflight-api-direct-api-openapi.yml
  format: yaml
  label: Automation Preflight API Direct API
  slug: automation-preflight-api-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-direct-api-openapi.yml
- filename: automation-preflight-api-health-api-openapi.yml
  format: yaml
  label: Automation Preflight API Health API
  slug: automation-preflight-api-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tinyopsstudio.com
  spf: true
hosts:
- cert_expires: Dec 26 04:53:55 2026 GMT
  host: tinyopsstudio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 04:53:55 2026 GMT
  host: preflight.tinyopsstudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Automation Preflight Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automation Preflight API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Automation Preflight API
provider_slug: automation-preflight-api
slug: automation-preflight-api-domain-security
source_filename: automation-preflight-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tinyopsstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 04:53:55 2026 GMT\n  hsts: false\n- host: preflight.tinyopsstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 04:53:55 2026 GMT\n  hsts: null\ndomains:\n- domain: tinyopsstudio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/security/automation-preflight-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automation
- Integration
- Developer Tools
- Readiness
- Testing
- URL Analysis
- Web Scraping
- Agent Tools
- Quality Assurance
- Site Audit
- A2A
---
