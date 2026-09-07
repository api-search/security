---
api_specs:
- filename: env0-agents-api-openapi.yml
  format: yaml
  label: Env0 Agents API
  slug: env0-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-agents-api-openapi.yml
- filename: env0-approvalpolicies-api-openapi.yml
  format: yaml
  label: Env0 ApprovalPolicies API
  slug: env0-approvalpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-approvalpolicies-api-openapi.yml
- filename: env0-configuration-api-openapi.yml
  format: yaml
  label: Env0 Configuration API
  slug: env0-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-configuration-api-openapi.yml
- filename: env0-deployments-api-openapi.yml
  format: yaml
  label: Env0 Deployments API
  slug: env0-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-deployments-api-openapi.yml
- filename: env0-environments-api-openapi.yml
  format: yaml
  label: Env0 Environments API
  slug: env0-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-environments-api-openapi.yml
- filename: env0-modules-api-openapi.yml
  format: yaml
  label: Env0 Modules API
  slug: env0-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-modules-api-openapi.yml
- filename: env0-organizations-api-openapi.yml
  format: yaml
  label: Env0 Organizations API
  slug: env0-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-organizations-api-openapi.yml
- filename: env0-projects-api-openapi.yml
  format: yaml
  label: Env0 Projects API
  slug: env0-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-projects-api-openapi.yml
- filename: env0-templates-api-openapi.yml
  format: yaml
  label: Env0 Templates API
  slug: env0-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-templates-api-openapi.yml
- filename: env0-users-api-openapi.yml
  format: yaml
  label: Env0 Users API
  slug: env0-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-users-api-openapi.yml
- filename: env0-webhooks-api-openapi.yml
  format: yaml
  label: Env0 Webhooks API
  slug: env0-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-webhooks-api-openapi.yml
certification_count: 1
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Env0 Trust Center
name_suffix: Trust Center
overview: Env0 maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Env0
provider_slug: env0
slug: env0-trust-center
source_filename: env0-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprobe: true\nurl: https://docs.envzero.com/guides/overview/security-overview\nnote: >-\n  env zero has NO dedicated trust centre. trust.env0.com and trust.envzero.com do not resolve;\n  https://www.envzero.com/security and /trust both return 404. What it publishes instead is a\n  single \"Security overview\" page inside the documentation, which does name a real attestation\n  and describe the architecture. That page is recorded here as the compliance surface.\ncertifications:\n- name: SOC 2 Type II\n  scope: entire service offering\n  latest_report_issued: '2025-11'\n  self_serve: false\n  availability: on request from your account manager\ncertifications_absent:\n- ISO 27001\n- ISO 27017\n- ISO 27018\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\n- FIPS 140\nsecurity_posture:\n  hosting: AWS\n  edge: API Gateway + CloudFront + WAF\n  account_isolation: multiple AWS accounts; separate development account\n  internal_access: AWS SSO with\
  \ MFA\n  encryption_in_transit: HTTPS / SSH only\n  encryption_at_rest: S3, RDS and DynamoDB encryption\n  sensitive_variables: encrypted and unavailable in UI, logs or API - including to env zero staff\n  deployment_isolation: single-use sandboxed Docker container per deployment, destroyed afterwards\n  base_image: node alpine\n  hybrid_option: self-hosted agent keeps secrets and IaC runs inside the customer's cloud account\n  ip_allowlisting: per-organization IPv4/IPv6 allowlist over UI logins, API keys and the Agent API\n  sso: SAML 2.0, Azure AD / Microsoft Entra ID, SCIM 2.0 provisioning\npublished_risk_register:\n  present: true\n  note: env zero publishes a \"Possible Exploits\" section naming risks it does NOT mitigate\n  risks:\n  - malicious code in a linked VCS repository exfiltrating data during PR plan operations\n  - malicious third-party Terraform providers/modules reaching state files and sensitive variables\n  - arbitrary code execution through custom flows, unvalidated\
  \ and unblocked at deployment time\nevidence:\n- source: https://docs.envzero.com/guides/overview/security-overview\n  status: 200\n  fetched: '2026-09-06'\n  keywords: [soc 2, soc 2 type ii, encryption, sandboxing, sso, scim, mfa]\n- source: https://www.envzero.com/security\n  status: 404\n  fetched: '2026-09-06'\n- source: https://www.envzero.com/trust\n  status: 404\n  fetched: '2026-09-06'\n- source: https://trust.envzero.com/\n  status: dns-nxdomain\n  fetched: '2026-09-06'\nvulnerability_disclosure:\n  present: false\n  note: >-\n    No security.txt on any of the eight hosts probed, no responsible-disclosure page, no bug\n    bounty programme on HackerOne, Bugcrowd or Intigriti, and no security@ address published.\n    The only published contact is support@env0.com. This is a real gap and the cheapest one on\n    this list for env zero to close - an RFC 9116 security.txt at\n    https://www.envzero.com/.well-known/security.txt naming a contact and a policy URL.\n  probed:\n  - {url:\
  \ 'https://www.envzero.com/.well-known/security.txt', status: 404}\n  - {url: 'https://envzero.com/.well-known/security.txt', status: 404}\n  - {url: 'https://www.env0.com/.well-known/security.txt', status: 404}\n  - {url: 'https://api.env0.com/.well-known/security.txt', status: 403}\n  - {url: 'https://docs.envzero.com/.well-known/security.txt', status: 404}\n  checked: '2026-09-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/security/env0-trust-center.yml
summary_line: SOC 2 Type II
tags:
- FinOps
- Infrastructure as Code
- DevOps
- Cloud
- Terraform
- OpenTofu
- Platform Engineering
- Cloud Governance
- Drift Detection
trust_url: https://docs.envzero.com/guides/overview/security-overview
---
