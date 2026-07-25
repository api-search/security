---
api_specs:
- filename: plerion-alerts-api-openapi.yml
  format: yaml
  label: Plerion Alerts API
  slug: plerion-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-alerts-api-openapi.yml
- filename: plerion-asset-groups-api-openapi.yml
  format: yaml
  label: Plerion Asset groups API
  slug: plerion-asset-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-asset-groups-api-openapi.yml
- filename: plerion-assets-api-openapi.yml
  format: yaml
  label: Plerion Assets API
  slug: plerion-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-assets-api-openapi.yml
- filename: plerion-audit-logs-api-openapi.yml
  format: yaml
  label: Plerion Audit logs API
  slug: plerion-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-audit-logs-api-openapi.yml
- filename: plerion-aws-integration-api-openapi.yml
  format: yaml
  label: Plerion AWS integration API
  slug: plerion-aws-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-aws-integration-api-openapi.yml
- filename: plerion-code-security-api-openapi.yml
  format: yaml
  label: Plerion Code security API
  slug: plerion-code-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-code-security-api-openapi.yml
- filename: plerion-compliance-frameworks-api-openapi.yml
  format: yaml
  label: Plerion Compliance frameworks API
  slug: plerion-compliance-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-compliance-frameworks-api-openapi.yml
- filename: plerion-findings-api-openapi.yml
  format: yaml
  label: Plerion Findings API
  slug: plerion-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-findings-api-openapi.yml
- filename: plerion-integrations-api-openapi.yml
  format: yaml
  label: Plerion Integrations API
  slug: plerion-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-integrations-api-openapi.yml
- filename: plerion-risks-api-openapi.yml
  format: yaml
  label: Plerion Risks API
  slug: plerion-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-risks-api-openapi.yml
- filename: plerion-tenant-api-openapi.yml
  format: yaml
  label: Plerion Tenant API
  slug: plerion-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-tenant-api-openapi.yml
- filename: plerion-vulnerabilities-api-openapi.yml
  format: yaml
  label: Plerion Vulnerabilities API
  slug: plerion-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-vulnerabilities-api-openapi.yml
- filename: plerion-well-architected-frameworks-api-openapi.yml
  format: yaml
  label: Plerion Well-Architected frameworks API
  slug: plerion-well-architected-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-well-architected-frameworks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plerion.com
  spf: true
hosts:
- cert_expires: Oct 15 00:00:01 2026 GMT
  host: plerion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plerion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plerion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plerion
provider_slug: plerion
slug: plerion-domain-security
source_filename: plerion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plerion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plerion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/security/plerion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cloud Security
- CSPM
- Cloud Workload Protection
- Vulnerability Management
- Compliance
- AI Security
- DevSecOps
- API
---
