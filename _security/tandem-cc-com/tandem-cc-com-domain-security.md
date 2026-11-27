---
api_specs:
- filename: tandem-cc-com-admin-api-openapi.yml
  format: yaml
  label: Tandem Admin API
  slug: tandem-cc-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-admin-api-openapi.yml
- filename: tandem-cc-com-attachments-api-openapi.yml
  format: yaml
  label: Tandem Attachments API
  slug: tandem-cc-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-attachments-api-openapi.yml
- filename: tandem-cc-com-conventions-api-openapi.yml
  format: yaml
  label: Tandem Conventions API
  slug: tandem-cc-com-conventions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-conventions-api-openapi.yml
- filename: tandem-cc-com-drafts-api-openapi.yml
  format: yaml
  label: Tandem Drafts API
  slug: tandem-cc-com-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-drafts-api-openapi.yml
- filename: tandem-cc-com-healthz-api-openapi.yml
  format: yaml
  label: Tandem Healthz API
  slug: tandem-cc-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-healthz-api-openapi.yml
- filename: tandem-cc-com-inbound-api-openapi.yml
  format: yaml
  label: Tandem Inbound API
  slug: tandem-cc-com-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-inbound-api-openapi.yml
- filename: tandem-cc-com-messages-api-openapi.yml
  format: yaml
  label: Tandem Messages API
  slug: tandem-cc-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-messages-api-openapi.yml
- filename: tandem-cc-com-oauth-api-openapi.yml
  format: yaml
  label: Tandem OAuth API
  slug: tandem-cc-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-oauth-api-openapi.yml
- filename: tandem-cc-com-ops-api-openapi.yml
  format: yaml
  label: Tandem Ops API
  slug: tandem-cc-com-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-ops-api-openapi.yml
- filename: tandem-cc-com-passkeys-api-openapi.yml
  format: yaml
  label: Tandem Passkeys API
  slug: tandem-cc-com-passkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-passkeys-api-openapi.yml
- filename: tandem-cc-com-preview-api-openapi.yml
  format: yaml
  label: Tandem Preview API
  slug: tandem-cc-com-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-preview-api-openapi.yml
- filename: tandem-cc-com-public-api-openapi.yml
  format: yaml
  label: Tandem Public API
  slug: tandem-cc-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-public-api-openapi.yml
- filename: tandem-cc-com-threads-api-openapi.yml
  format: yaml
  label: Tandem Threads API
  slug: tandem-cc-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-threads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tandem-cc.com
  spf: true
hosts:
- cert_expires: May 17 15:59:00 2027 GMT
  host: tandem-cc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tandem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tandem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tandem
provider_slug: tandem-cc-com
slug: tandem-cc-com-domain-security
source_filename: tandem-cc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tandem-cc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 17 15:59:00 2027 GMT\n  hsts: null\ndomains:\n- domain: tandem-cc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tandem-cc-com/security/tandem-cc-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Communication
- Collaboration
- MCP
---
