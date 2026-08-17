---
api_specs:
- filename: rudderstack-event-streaming-asyncapi.yml
  format: yaml
  label: RudderStack Webhook Source API
  slug: rudderstack-webhook-source-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/asyncapi/rudderstack-event-streaming-asyncapi.yml
- filename: rudderstack-http-api-api-openapi.yml
  format: yaml
  label: RudderStack HTTP API API
  slug: rudderstack-http-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-http-api-api-openapi.yml
- filename: rudderstack-internal-api-api-openapi.yml
  format: yaml
  label: RudderStack Internal API API
  slug: rudderstack-internal-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-internal-api-api-openapi.yml
certifications:
- SOC 2
- HIPAA
- GDPR
description: 'RudderStack publishes a security and compliance overview page rather than a hosted trust center — there is no trust.rudderstack.com (DNS does not resolve) and no Vanta/Drata/SafeBase portal was found. The page names three compliance programs and the enterprise security controls that back them. The architectural claim it leads with is material to how the compliance posture works: RudderStack is warehouse-native and states it does not store customer data, so much of the data-at-rest control surface belongs to the customer''s own warehouse.'
kind: trust-center
layout: security
name: Rudderstack Trust Center
name_suffix: Trust Center
overview: RudderStack maintains a public trust center documenting SOC 2, HIPAA, and GDPR compliance.
provider_name: RudderStack
provider_slug: rudderstack
slug: rudderstack-trust-center
source_filename: rudderstack-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://www.rudderstack.com/security/\nurl: https://www.rudderstack.com/security/\nhttp_status: 200\ndescription: >-\n  RudderStack publishes a security and compliance overview page rather than a\n  hosted trust center — there is no trust.rudderstack.com (DNS does not resolve)\n  and no Vanta/Drata/SafeBase portal was found. The page names three compliance\n  programs and the enterprise security controls that back them. The architectural\n  claim it leads with is material to how the compliance posture works:\n  RudderStack is warehouse-native and states it does not store customer data, so\n  much of the data-at-rest control surface belongs to the customer's own warehouse.\ntrust_center_hosted: false\nprobed:\n  - {url: 'https://trust.rudderstack.com/', status: 'DNS did not resolve'}\n  - {url: 'https://security.rudderstack.com/', status: 'DNS did not resolve'}\n  - {url: 'https://www.rudderstack.com/security/',\
  \ status: 200}\ncertifications:\n  - name: SOC 2\n    level: Type 2\n    status: obtained\n    evidence: >-\n      \"SOC 2 - We have obtained SOC 2 Type 2 compliance and regularly audit our\n      policies and procedures to ensure continued compliance.\"\n  - name: HIPAA\n    status: compliant, BAA available\n    plan_gate: Enterprise\n    evidence: >-\n      \"HIPAA - We comply with HIPAA requirements for PHI and can sign a BAA.\"\n      The pricing comparison table lists HIPAA / BAA under Enterprise only.\n  - name: GDPR\n    status: compliant\n    evidence: >-\n      \"GDPR - We compliant with GDPR and are constantly adding features to enable\n      you to meet your EU data protection requirements.\" EU data residency is\n      backed by a separate control-plane host, https://api.eu.rudderstack.com.\nnot_claimed:\n  certifications:\n    - ISO 27001\n    - PCI DSS\n    - FedRAMP\n    - CSA STAR\n  note: >-\n    These were not claimed on the security page. That records the absence of\
  \ a\n    published claim, not a finding about RudderStack's controls.\nsecurity_controls_published:\n  - {name: SSO, detail: 'Okta, OneLogin', plan_gate: Enterprise}\n  - {name: SSH Tunnel, detail: Encryption for in-flight data to warehouses/databases, plan_gate: Enterprise}\n  - {name: Permissions management, detail: Limit access to features exposing PHI or PII}\n  - {name: Audit logs, detail: 'Track user activity in the workspace; exposed programmatically via the Audit Logs API (/v2/audit-logs)'}\n  - {name: MFA, detail: 'TOTP authenticator app or SMS, with single-use backup codes', since: '2026-08-05'}\n  - {name: VPC deployment, detail: Available on Enterprise (talk to sales)}\n  - {name: PII masking, detail: Data Compliance Toolkit; also applied automatically by Rudder AI}\n  - {name: User suppression and deletion, detail: 'User Suppression API (/v2/regulations)', plan_gate: 'Growth, Enterprise'}\narchitecture_claim: >-\n  \"We do not store your data, giving you complete ownership,\
  \ control and\n  transparency. We build on your warehouse.\"\nrelated:\n  vulnerability_disclosure: security/rudderstack-vulnerability-disclosure.yml\n  domain_security: security/rudderstack-domain-security.yml\n  legal:\n    master_service_agreement: https://www.rudderstack.com/master-service-agreement/\n    privacy_policy: https://www.rudderstack.com/privacy-policy/\n    terms_of_service: https://www.rudderstack.com/terms-of-service/\nevidence:\n  - source: https://www.rudderstack.com/security/\n    http_status: 200\n    keywords:\n      - soc 2\n      - soc 2 type 2\n      - hipaa\n      - baa\n      - gdpr\n      - sso\n      - audit logs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/security/rudderstack-trust-center.yml
summary_line: SOC 2, HIPAA, GDPR
tags:
- Customer Data Platform
- CDP
- Data Pipeline
- Open Source
- Event Streaming
- Reverse ETL
- Analytics
- Identity Resolution
trust_url: https://www.rudderstack.com/security/
---
