---
api_specs:
- filename: axuall-actor-api-openapi.yml
  format: yaml
  label: Axuall Actor API
  slug: axuall-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-actor-api-openapi.yml
- filename: axuall-address-deduplications-api-openapi.yml
  format: yaml
  label: Axuall Address Deduplications API
  slug: axuall-address-deduplications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-address-deduplications-api-openapi.yml
- filename: axuall-agent-api-openapi.yml
  format: yaml
  label: Axuall Agent API
  slug: axuall-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-agent-api-openapi.yml
- filename: axuall-authentication-api-openapi.yml
  format: yaml
  label: Axuall Authentication API
  slug: axuall-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-authentication-api-openapi.yml
- filename: axuall-case-log-artifact-api-openapi.yml
  format: yaml
  label: Axuall Case Log Artifact API
  slug: axuall-case-log-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-case-log-artifact-api-openapi.yml
- filename: axuall-documents-api-openapi.yml
  format: yaml
  label: Axuall Documents API
  slug: axuall-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-documents-api-openapi.yml
- filename: axuall-email-api-openapi.yml
  format: yaml
  label: Axuall Email API
  slug: axuall-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-email-api-openapi.yml
- filename: axuall-facilities-api-openapi.yml
  format: yaml
  label: Axuall Facilities API
  slug: axuall-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-facilities-api-openapi.yml
- filename: axuall-fsmb-artifact-api-openapi.yml
  format: yaml
  label: Axuall FSMB Artifact API
  slug: axuall-fsmb-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-fsmb-artifact-api-openapi.yml
- filename: axuall-invite-api-openapi.yml
  format: yaml
  label: Axuall Invite API
  slug: axuall-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-invite-api-openapi.yml
- filename: axuall-monitoring-reports-api-openapi.yml
  format: yaml
  label: Axuall Monitoring reports API
  slug: axuall-monitoring-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-monitoring-reports-api-openapi.yml
- filename: axuall-provider-preview-api-openapi.yml
  format: yaml
  label: Axuall Provider Preview API
  slug: axuall-provider-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-provider-preview-api-openapi.yml
- filename: axuall-providers-api-openapi.yml
  format: yaml
  label: Axuall Providers API
  slug: axuall-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-providers-api-openapi.yml
- filename: axuall-recipes-api-openapi.yml
  format: yaml
  label: Axuall Recipes API
  slug: axuall-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-recipes-api-openapi.yml
- filename: axuall-tasks-api-openapi.yml
  format: yaml
  label: Axuall Tasks API
  slug: axuall-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axuall.com
  spf: true
hosts:
- cert_expires: Dec  1 21:31:42 2026 GMT
  host: axuall.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axuall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axuall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axuall
provider_slug: axuall
slug: axuall-domain-security
source_filename: axuall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axuall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 21:31:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axuall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/security/axuall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Data
- Credentialing
- AI
---
