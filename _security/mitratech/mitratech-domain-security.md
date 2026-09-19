---
api_specs:
- filename: mitratech-dashboard-api-openapi.yml
  format: yaml
  label: Mitratech Dashboard API
  slug: mitratech-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-dashboard-api-openapi.yml
- filename: mitratech-files-api-openapi.yml
  format: yaml
  label: Mitratech Files API
  slug: mitratech-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-files-api-openapi.yml
- filename: mitratech-gridconfigurations-api-openapi.yml
  format: yaml
  label: Mitratech Grid Configurations API
  slug: mitratech-gridconfigurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-gridconfigurations-api-openapi.yml
- filename: mitratech-templates-api-openapi.yml
  format: yaml
  label: Mitratech Templates API
  slug: mitratech-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-templates-api-openapi.yml
- filename: mitratech-users-api-openapi.yml
  format: yaml
  label: Mitratech Users API
  slug: mitratech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-users-api-openapi.yml
- filename: mitratech-workflow-api-openapi.yml
  format: yaml
  label: Mitratech Workflow API
  slug: mitratech-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-workflow-api-openapi.yml
- filename: mitratech-workflows-api-openapi.yml
  format: yaml
  label: Mitratech Workflows API
  slug: mitratech-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-workflows-api-openapi.yml
- filename: mitratech-health-check-api-openapi.yml
  format: yaml
  label: Mitratech Health Check API
  slug: mitratech-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-health-check-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "comococa.com"
  - 0 issue "awstrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mitratech.com
  spf: true
hosts:
- cert_expires: Nov 12 15:36:48 2026 GMT
  host: mitratech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: success.mitratech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Mitratech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitratech, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mitratech
provider_slug: mitratech
slug: mitratech-domain-security
source_filename: mitratech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mitratech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 15:36:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: success.mitratech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mitratech.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comococa.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/security/mitratech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Legal Operations
- Enterprise Legal Management
- Matter Management
- Governance Risk and Compliance
- Compliance
- Workflow-Automation
- Contract Lifecycle Management
- HR Compliance
- Risk Management
- Immigration
- OData
- MCP
---
