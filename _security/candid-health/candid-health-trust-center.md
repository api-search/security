---
api_specs:
- filename: candid-health-default-api-openapi.yml
  format: yaml
  label: Candid Health Default API
  slug: candid-health-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-default-api-openapi.yml
- filename: candid-health-diagnoses-api-openapi.yml
  format: yaml
  label: Candid Health Diagnoses API
  slug: candid-health-diagnoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-diagnoses-api-openapi.yml
- filename: candid-health-v1-api-openapi.yml
  format: yaml
  label: Candid Health V1 API
  slug: candid-health-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v1-api-openapi.yml
- filename: candid-health-v2-api-openapi.yml
  format: yaml
  label: Candid Health V2 API
  slug: candid-health-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v2-api-openapi.yml
- filename: candid-health-v3-api-openapi.yml
  format: yaml
  label: Candid Health V3 API
  slug: candid-health-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v3-api-openapi.yml
- filename: candid-health-v4-api-openapi.yml
  format: yaml
  label: Candid Health V4 API
  slug: candid-health-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/openapi/candid-health-v4-api-openapi.yml
certifications:
- SOC 2 Type 2
- SOC 2 Type 1
- SOC 1 Type 1
- HIPAA (Business Associate)
description: Candid Health operates a Drata-hosted trust center at trust.joincandidhealth.com. It is provisioned and live but sits behind a Cloudflare bot challenge, so its contents could not be read anonymously — the certifications recorded below come from Candid's own newsroom posts, each naming the report, the period and the auditing firm, not from the trust page itself.
kind: trust-center
layout: security
name: Candid Health Trust Center
name_suffix: Trust Center
overview: Candid Health maintains a public trust center documenting SOC 2 Type 2, SOC 2 Type 1, SOC 1 Type 1, and HIPAA (Business Associate) compliance.
provider_name: Candid Health
provider_slug: candid-health
slug: candid-health-trust-center
source_filename: candid-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nprobe: true\nsource: https://trust.joincandidhealth.com/\nname: Candid Health Trust Center\ndescription: >-\n  Candid Health operates a Drata-hosted trust center at trust.joincandidhealth.com.\n  It is provisioned and live but sits behind a Cloudflare bot challenge, so its\n  contents could not be read anonymously — the certifications recorded below come\n  from Candid's own newsroom posts, each naming the report, the period and the\n  auditing firm, not from the trust page itself.\nurl: https://trust.joincandidhealth.com/\nplatform: Drata\nplatform_evidence: 'DNS: trust.joincandidhealth.com CNAME trust.cname.drata.com'\nreadable_anonymously: false\n\ncertifications:\n  - name: SOC 2 Type 2\n    criteria: [Security, Availability, Confidentiality]\n    period: 2025-01-15 to 2025-04-15\n    opinion: unqualified\n    auditor: AssurancePoint, LLC\n    source: https://candidhealth.com/blog/candid-health-successfully-completed-type-2-soc-2-examination-with-an-unqualified-opinion\n\
  \  - name: SOC 2 Type 1\n    opinion: unqualified\n    auditor: AssurancePoint, LLC\n    source: https://candidhealth.com/blog/candid-health-successfully-completed-type-1-soc-2-examination-with-an-unqualified-opinion\n  - name: SOC 1 Type 1\n    as_of: '2025-12-31'\n    opinion: clean\n    auditor: AssurancePoint, LLC\n    scope: >-\n      Claims and Payment Interface Processing, Invalid Claims and Interface Error\n      Handling, Account Balances, Billing, Data Communications, Logical Access,\n      Change Management.\n    source: https://candidhealth.com/blog/candid-health-achieves-type-1-soc-1-certification-with-clean-auditor-opinion\n  - name: HIPAA (Business Associate)\n    basis: contractual — BAAs with customers; PHI prohibited in the Sandbox environment\n    source: https://candidhealth.com/privacy-policy\n\nnot_claimed:\n  - ISO 27001\n  - HITRUST CSF\n  - PCI DSS\n  - FedRAMP\n\nreport_access:\n  self_serve_download: unknown\n  note: >-\n    Drata trust centers normally gate\
  \ SOC reports behind an NDA click-through. Whether\n    Candid's does could not be established without passing the bot challenge.\n\nx-evidence:\n  - url: https://trust.joincandidhealth.com/\n    http_status: 403\n    detail: >-\n      Cloudflare managed challenge (cf-mitigated: challenge, server: cloudflare). The host\n      resolves, serves TLS with HSTS preload, and CNAMEs to trust.cname.drata.com — so the\n      trust center exists and is provisioned; it is simply not machine-readable.\n  - url: https://candidhealth.com/blog/candid-health-successfully-completed-type-2-soc-2-examination-with-an-unqualified-opinion\n    http_status: 200\n  - url: https://candidhealth.com/blog/candid-health-achieves-type-1-soc-1-certification-with-clean-auditor-opinion\n    http_status: 200\n  - dns: trust.joincandidhealth.com\n    record: CNAME\n    value: trust.cname.drata.com\n\nnotes:\n  - >-\n    The trust center is on joincandidhealth.com while the marketing site and the audit\n    announcements\
  \ are on candidhealth.com. Both domains belong to Candid Health — the\n    newer candidhealth.com Nuxt site links to app.joincandidhealth.com and the older\n    joincandidhealth.com Webflow site links to candidhealth.com — but a buyer following\n    the newer brand domain will not find the trust center, because nothing on\n    candidhealth.com links to it.\n  - >-\n    No vulnerability disclosure program, bug bounty, or security.txt was found on any\n    host, so no VulnerabilityDisclosure artifact is written and no Security pointer is\n    emitted. For a HIPAA business associate handling PHI at this scale, a published\n    disclosure channel is the most obvious missing piece of the security posture.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candid-health/refs/heads/main/security/candid-health-trust-center.yml
summary_line: SOC 2 Type 2, SOC 2 Type 1, SOC 1 Type 1, HIPAA (Business Associate)
tags:
- Medical Billing
- Revenue Cycle Management
- Healthcare
- Claims
- Eligibility
- Prior Authorization
- Remittance
- Patient Collections
- Credentialing
- Insurance
trust_url: https://trust.joincandidhealth.com/
---
