---
api_specs:
- filename: budibase-applications-api-openapi.yml
  format: yaml
  label: Budibase Applications API
  slug: budibase-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-applications-api-openapi.yml
- filename: budibase-queries-api-openapi.yml
  format: yaml
  label: Budibase Queries API
  slug: budibase-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-queries-api-openapi.yml
- filename: budibase-rows-api-openapi.yml
  format: yaml
  label: Budibase Rows API
  slug: budibase-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-rows-api-openapi.yml
- filename: budibase-tables-api-openapi.yml
  format: yaml
  label: Budibase Tables API
  slug: budibase-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-tables-api-openapi.yml
- filename: budibase-users-api-openapi.yml
  format: yaml
  label: Budibase Users API
  slug: budibase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-users-api-openapi.yml
- filename: budibase-public-api-openapi.yml
  format: yaml
  label: Budibase Public API
  slug: budibase-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-public-api-openapi.yml
certification_count: 3
certifications:
- ISO 27001
- GDPR
- SOC 1 / SOC 2
description: Budibase publishes a security page rather than a dedicated trust center — there is no trust.budibase.com (NXDOMAIN, probed 2026-09-04) and no document portal. The page states certifications, hosting geography, encryption posture and an audit cadence, but offers no downloadable evidence and no subprocessor list.
kind: trust-center
layout: security
name: Budibase Trust Center
name_suffix: Trust Center
overview: Budibase maintains a public trust center documenting ISO 27001, GDPR, and SOC 1 / SOC 2 compliance.
provider_name: Budibase
provider_slug: budibase
slug: budibase-trust-center
source_filename: budibase-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nprobe: true\nsource: https://budibase.com/security\nurl: https://budibase.com/security\nstatus: 200\nverified: '2026-09-04'\ndescription: >-\n  Budibase publishes a security page rather than a dedicated trust center — there is no\n  trust.budibase.com (NXDOMAIN, probed 2026-09-04) and no document portal. The page states\n  certifications, hosting geography, encryption posture and an audit cadence, but offers no\n  downloadable evidence and no subprocessor list.\ncertifications:\n  - name: ISO 27001\n    claimed: true\n    scope: Budibase\n    evidence: >-\n      \"ISO 27001 Certified\" in the site footer; \"ISO 27001 — Enterprise-grade security\n      certifications to meet your compliance requirements\" on the security page.\n    report_available: false\n  - name: GDPR\n    claimed: true\n    scope: Budibase\n    evidence: '\"GDPR Compliant\" stated in the site footer.'\n    report_available: false\n  - name: SOC 1 / SOC 2\n    claimed:\
  \ false\n    scope: infrastructure provider only\n    evidence: >-\n      The page says servers are \"hosted within the EU (Ireland) in data centers certified\n      by SOC 1/2 and ISO 27001\". That certifies the DATA CENTRE, not Budibase. Budibase\n      makes no SOC 2 claim of its own — recorded here so the inherited wording is not\n      misread as a Budibase attestation.\n    report_available: false\nsecurity_posture:\n  hosting_region: EU (Ireland)\n  data_in_transit: TLS 1.3, mandatory HTTPS\n  data_at_rest: AES-256\n  penetration_testing: >-\n    \"Annual penetration tests and AWS security configuration audits from 3rd party\n    vendors.\"\n  self_hosting: >-\n    Open source, deployable via Kubernetes, Docker and more, including air-gapped\n    deployments — the strongest data-sovereignty answer in this artifact.\nplatform_security_features:\n  source: https://budibase.com/security and https://budibase.com/pricing.json\n  features:\n  - name: RBAC\n    detail: Control the data\
  \ and resources users can access. Also governs Public API key privileges.\n  - name: SSO\n    detail: Integrates with auth tools including OpenID Connect. Available on every plan.\n  - name: Enforceable SSO\n    detail: Business tier and above.\n  - name: Audit logs\n    detail: Comprehensive audit trails for user actions and system events. Enterprise tier only.\n  - name: SCIM / Active Directory sync\n    detail: Enterprise tier only.\n  - name: Environment variables\n    detail: Secure handling of database credentials and API keys across the platform.\n  - name: User groups\n    detail: Simplifies managing user access to apps.\ngaps:\n  - No dedicated trust portal; trust.budibase.com does not resolve.\n  - No downloadable ISO 27001 certificate or audit summary, and no NDA-gated document room.\n  - No published subprocessor list or data-processing addendum link on the security page.\n  - No /.well-known/security.txt on any host — see security/budibase-vulnerability-disclosure.yml.\nevidence:\n\
  \  - source: https://budibase.com/security\n    status: 200\n    keywords:\n      - iso 27001\n      - gdpr\n      - tls 1.3\n      - aes256\n      - penetration tests\n      - air-gapped\n  - source: https://trust.budibase.com\n    status: 0\n    result: DNS does not resolve (NXDOMAIN)\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/security/budibase-trust-center.yml
summary_line: ISO 27001, GDPR, SOC 1 / SOC 2
tags:
- AI Agents
- Automation
- Internal Tools
- Low-Code
- Open-Source
- Workflow-Automation
trust_url: https://budibase.com/security
---
