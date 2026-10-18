---
api_specs:
- filename: coreview-connect-api-openapi.yml
  format: yaml
  label: CoreView Connect API
  slug: coreview-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coreview/refs/heads/main/openapi/coreview-connect-api-openapi.yml
- filename: coreview-public-api-openapi.yml
  format: yaml
  label: CoreView Public API
  slug: coreview-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coreview/refs/heads/main/openapi/coreview-public-api-openapi.yml
- filename: coreview-teams-api-openapi.yml
  format: yaml
  label: CoreView Teams API
  slug: coreview-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coreview/refs/heads/main/openapi/coreview-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coreview.com
  spf: true
hosts:
- cert_expires: Dec 12 15:15:09 2026 GMT
  host: www.coreview.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coreview Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreView, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CoreView
provider_slug: coreview
slug: coreview-domain-security
source_filename: coreview-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coreview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:15:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coreview.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coreview/refs/heads/main/security/coreview-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microsoft 365
- Tenant Resilience
- Configuration Management
- Identity Security
- License Optimization
- SharePoint Control
- Enterprise Saas
---
