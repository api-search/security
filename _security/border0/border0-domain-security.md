---
api_specs:
- filename: border0-audit-actions-api-openapi.yml
  format: yaml
  label: Border0 Audit Actions API
  slug: border0-audit-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-audit-actions-api-openapi.yml
- filename: border0-client-api-openapi.yml
  format: yaml
  label: Border0 Client API
  slug: border0-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-client-api-openapi.yml
- filename: border0-connect-api-openapi.yml
  format: yaml
  label: Border0 Connect API
  slug: border0-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-connect-api-openapi.yml
- filename: border0-login-api-openapi.yml
  format: yaml
  label: Border0 Login API
  slug: border0-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-login-api-openapi.yml
- filename: border0-mtls-ca-api-openapi.yml
  format: yaml
  label: Border0 Mtls-Ca API
  slug: border0-mtls-ca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-mtls-ca-api-openapi.yml
- filename: border0-organization-api-openapi.yml
  format: yaml
  label: Border0 Organization API
  slug: border0-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-organization-api-openapi.yml
- filename: border0-organizations-api-openapi.yml
  format: yaml
  label: Border0 Organizations API
  slug: border0-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-organizations-api-openapi.yml
- filename: border0-policies-api-openapi.yml
  format: yaml
  label: Border0 Policies API
  slug: border0-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-policies-api-openapi.yml
- filename: border0-policy-api-openapi.yml
  format: yaml
  label: Border0 Policy API
  slug: border0-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-policy-api-openapi.yml
- filename: border0-session-api-openapi.yml
  format: yaml
  label: Border0 Session API
  slug: border0-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-session-api-openapi.yml
- filename: border0-sessions-api-openapi.yml
  format: yaml
  label: Border0 Sessions API
  slug: border0-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-sessions-api-openapi.yml
- filename: border0-socket-api-openapi.yml
  format: yaml
  label: Border0 Socket API
  slug: border0-socket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-socket-api-openapi.yml
- filename: border0-stats-api-openapi.yml
  format: yaml
  label: Border0 Stats API
  slug: border0-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-stats-api-openapi.yml
- filename: border0-user-api-openapi.yml
  format: yaml
  label: Border0 User API
  slug: border0-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-user-api-openapi.yml
- filename: border0-users-api-openapi.yml
  format: yaml
  label: Border0 Users API
  slug: border0-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: border0.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.border0.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Border0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Border0, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Border0
provider_slug: border0
slug: border0-domain-security
source_filename: border0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.border0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: border0.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/security/border0-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Zero Trust
- Network Access
- Security
- Identity and Access Management
- Infrastructure
- VPN
- SSH
- Databases
- Kubernetes
- Company
---
