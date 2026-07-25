---
api_specs:
- filename: nexthink-campaigns-api-openapi.yml
  format: yaml
  label: Nexthink Campaigns API
  slug: nexthink-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-campaigns-api-openapi.yml
- filename: nexthink-device-deletions-api-openapi.yml
  format: yaml
  label: Nexthink device-deletions API
  slug: nexthink-device-deletions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-device-deletions-api-openapi.yml
- filename: nexthink-enrichment-api-openapi.yml
  format: yaml
  label: Nexthink enrichment API
  slug: nexthink-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-enrichment-api-openapi.yml
- filename: nexthink-execute-api-openapi.yml
  format: yaml
  label: Nexthink Execute API
  slug: nexthink-execute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-execute-api-openapi.yml
- filename: nexthink-export-api-openapi.yml
  format: yaml
  label: Nexthink Export API
  slug: nexthink-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-export-api-openapi.yml
- filename: nexthink-handoff-api-api-openapi.yml
  format: yaml
  label: Nexthink Handoff API API
  slug: nexthink-handoff-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-handoff-api-api-openapi.yml
- filename: nexthink-remote-actions-api-openapi.yml
  format: yaml
  label: Nexthink Remote actions API
  slug: nexthink-remote-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-remote-actions-api-openapi.yml
- filename: nexthink-workflows-api-openapi.yml
  format: yaml
  label: Nexthink Workflows API
  slug: nexthink-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nexthink.com
  spf: true
hosts:
- cert_expires: Sep 19 15:32:18 2026 GMT
  host: nexthink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexthink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexthink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nexthink
provider_slug: nexthink
slug: nexthink-domain-security
source_filename: nexthink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexthink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:32:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexthink.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/security/nexthink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Digital Employee Experience
- Endpoint Analytics
- IT Operations
- Automation
- Observability
- DEX
---
