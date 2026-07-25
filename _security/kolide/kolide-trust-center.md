---
api_specs:
- filename: kolide-admin-users-api-openapi.yml
  format: yaml
  label: Kolide Admin Users API
  slug: kolide-admin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-admin-users-api-openapi.yml
- filename: kolide-audit-logs-api-openapi.yml
  format: yaml
  label: Kolide Audit Logs API
  slug: kolide-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-audit-logs-api-openapi.yml
- filename: kolide-auth-logs-api-openapi.yml
  format: yaml
  label: Kolide Auth Logs API
  slug: kolide-auth-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-auth-logs-api-openapi.yml
- filename: kolide-checks-api-openapi.yml
  format: yaml
  label: Kolide Checks API
  slug: kolide-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-checks-api-openapi.yml
- filename: kolide-custom-check-drafts-api-openapi.yml
  format: yaml
  label: Kolide Custom Check Drafts API
  slug: kolide-custom-check-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-custom-check-drafts-api-openapi.yml
- filename: kolide-deprovisioned-people-api-openapi.yml
  format: yaml
  label: Kolide Deprovisioned People API
  slug: kolide-deprovisioned-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-deprovisioned-people-api-openapi.yml
- filename: kolide-device-groups-api-openapi.yml
  format: yaml
  label: Kolide Device Groups API
  slug: kolide-device-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-device-groups-api-openapi.yml
- filename: kolide-devices-api-openapi.yml
  format: yaml
  label: Kolide Devices API
  slug: kolide-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-devices-api-openapi.yml
- filename: kolide-exemption-requests-api-openapi.yml
  format: yaml
  label: Kolide Exemption Requests API
  slug: kolide-exemption-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-exemption-requests-api-openapi.yml
- filename: kolide-issues-api-openapi.yml
  format: yaml
  label: Kolide Issues API
  slug: kolide-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-issues-api-openapi.yml
- filename: kolide-live-query-campaigns-api-openapi.yml
  format: yaml
  label: Kolide Live Query Campaigns API
  slug: kolide-live-query-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-live-query-campaigns-api-openapi.yml
- filename: kolide-packages-api-openapi.yml
  format: yaml
  label: Kolide Packages API
  slug: kolide-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-packages-api-openapi.yml
- filename: kolide-people-api-openapi.yml
  format: yaml
  label: Kolide People API
  slug: kolide-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-people-api-openapi.yml
- filename: kolide-person-groups-api-openapi.yml
  format: yaml
  label: Kolide Person Groups API
  slug: kolide-person-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-person-groups-api-openapi.yml
- filename: kolide-registration-requests-api-openapi.yml
  format: yaml
  label: Kolide Registration Requests API
  slug: kolide-registration-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-registration-requests-api-openapi.yml
- filename: kolide-reporting-api-openapi.yml
  format: yaml
  label: Kolide Reporting API
  slug: kolide-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-reporting-api-openapi.yml
- filename: kolide-whoami-api-openapi.yml
  format: yaml
  label: Kolide Whoami API
  slug: kolide-whoami-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-whoami-api-openapi.yml
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Kolide Trust Center
name_suffix: Trust Center
overview: Kolide maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Kolide
provider_slug: kolide
slug: kolide-trust-center
source_filename: kolide-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.kolide.com/security\nurl: https://www.kolide.com/security\nnotes: >-\n  Kolide does not run a dedicated trust-center subdomain (no trust.kolide.com). Its\n  security and compliance posture is published on the /security page plus dedicated legal\n  pages. Kolide is part of 1Password Extended Access Management and shares 1Password's\n  status page.\ncertifications:\n- name: SOC 2 Type II\n  url: https://www.kolide.com/legal/soc2\n- name: GDPR\n  url: https://www.kolide.com/legal/gdpr\nnot_claimed:\n- ISO/IEC 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\npractices:\n  encryption_in_transit: HTTPS/TLS 256-bit for all traffic\n  encryption_at_rest: AES-256\n  audit_logs: Customer-accessible audit logs (GET /audit_logs)\n  penetration_testing: >-\n    Engages professional compliance auditors, penetration testers and independent\n    security researchers.\n  vulnerability_scanning: Automated\n  code_review: Continuous\
  \ review as part of the deployment model\n  transparency: >-\n    \"Honesty and Transparency by Default\" — the agent source is open\n    (github.com/kolide/launcher) and end users get a Privacy Center showing what is\n    collected about their device.\nrelated:\n  vulnerability_disclosure: kolide-vulnerability-disclosure.yml\n  domain_security: kolide-domain-security.yml\n  status_page: https://status.1password.com\n  privacy_policy: https://www.kolide.com/legal/privacy\n  terms: https://www.kolide.com/legal/terms\n  api_terms: https://1password.com/legal/api-sdk-terms-of-service\nevidence:\n- source: https://www.kolide.com/security\n  keywords:\n  - soc2\n  - gdpr\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/security/kolide-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Company
- B2B
- Security
- Device Trust
- Endpoint Security
- Zero Trust
- Compliance
- Identity
- osquery
- Device Management
trust_url: https://www.kolide.com/security
---
