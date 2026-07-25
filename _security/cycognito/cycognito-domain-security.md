---
api_specs:
- filename: cycognito-assets-api-openapi.yml
  format: yaml
  label: CyCognito Assets API
  slug: cycognito-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-assets-api-openapi.yml
- filename: cycognito-audit-logs-api-openapi.yml
  format: yaml
  label: CyCognito Audit Logs API
  slug: cycognito-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-audit-logs-api-openapi.yml
- filename: cycognito-cloud-connectors-api-openapi.yml
  format: yaml
  label: CyCognito Cloud Connectors API
  slug: cycognito-cloud-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-cloud-connectors-api-openapi.yml
- filename: cycognito-export-data-api-openapi.yml
  format: yaml
  label: CyCognito Export Data API
  slug: cycognito-export-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-export-data-api-openapi.yml
- filename: cycognito-issues-api-openapi.yml
  format: yaml
  label: CyCognito Issues API
  slug: cycognito-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-issues-api-openapi.yml
- filename: cycognito-organizations-api-openapi.yml
  format: yaml
  label: CyCognito Organizations API
  slug: cycognito-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-organizations-api-openapi.yml
- filename: cycognito-realm-api-openapi.yml
  format: yaml
  label: CyCognito Realm API
  slug: cycognito-realm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-realm-api-openapi.yml
- filename: cycognito-reports-api-openapi.yml
  format: yaml
  label: CyCognito Reports API
  slug: cycognito-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-reports-api-openapi.yml
- filename: cycognito-revalidation-api-openapi.yml
  format: yaml
  label: CyCognito Revalidation API
  slug: cycognito-revalidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-revalidation-api-openapi.yml
- filename: cycognito-scope-management-api-openapi.yml
  format: yaml
  label: CyCognito Scope Management API
  slug: cycognito-scope-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-scope-management-api-openapi.yml
- filename: cycognito-users-api-openapi.yml
  format: yaml
  label: CyCognito Users API
  slug: cycognito-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-users-api-openapi.yml
- filename: cycognito-verify-ips-api-openapi.yml
  format: yaml
  label: CyCognito Verify IPs API
  slug: cycognito-verify-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-verify-ips-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cycognito.com
  spf: true
hosts:
- cert_expires: Oct 11 11:31:18 2026 GMT
  host: www.cycognito.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cycognito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyCognito, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CyCognito
provider_slug: cycognito
slug: cycognito-domain-security
source_filename: cycognito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cycognito.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 11:31:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cycognito.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/security/cycognito-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Attack Surface Management
- Exposure Management
- Security
- Vulnerability Management
- Cloud Security
- API Security
---
