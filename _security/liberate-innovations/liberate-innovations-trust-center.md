---
api_specs:
- filename: liberate-innovations-orchestration-openapi.yml
  format: yaml
  label: Liberate Orchestration Platform API
  slug: orchestration-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberate-innovations/refs/heads/main/openapi/liberate-innovations-orchestration-openapi.yml
certifications:
- SOC 2
- HIPAA
- PCI DSS
- GDPR
- CCPA
- ISO 27001
- FedRAMP
description: Liberate publishes a dedicated security page naming its compliance certifications and links out to a hosted Vanta trust center. Because Liberate sells into insurance carriers and agencies and handles claims data over voice, its published posture leans on HIPAA, SOC 2, and PCI DSS.
kind: trust-center
layout: security
name: Liberate Innovations Trust Center
name_suffix: Trust Center
overview: Liberate Innovations maintains a public trust center documenting SOC 2, HIPAA, PCI DSS, GDPR, CCPA, ISO 27001, and FedRAMP compliance.
provider_name: Liberate Innovations
provider_slug: liberate-innovations
slug: liberate-innovations-trust-center
source_filename: liberate-innovations-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.liberateinc.com/security\nname: Liberate trust center\ndescription: >-\n  Liberate publishes a dedicated security page naming its compliance certifications and links out to\n  a hosted Vanta trust center. Because Liberate sells into insurance carriers and agencies and\n  handles claims data over voice, its published posture leans on HIPAA, SOC 2, and PCI DSS.\n\ntrust_center:\n  published: true\n  url: https://app.vanta.com/liberateinc.com/trust/a3f4px3jh3gd2prixhl6\n  platform: Vanta\n  status: 200\n  public_access: true\n  note: >-\n    The Vanta-hosted trust center renders client-side, so the certification list below was read from\n    Liberate's own security page rather than scraped from the trust center document. Report\n    downloads on Vanta trust centers are typically gated behind an NDA request.\n\nsecurity_page:\n  url: https://www.liberateinc.com/security\n  status: 200\n\ncertifications:\n  - name: SOC\
  \ 2\n    claimed: true\n    type: not specified (Type I vs Type II not stated publicly)\n    evidence: >-\n      \"Liberate provides enterprise-grade security with certifications in HIPAA, SOC 2, PCI, and\n      GDPR\" and \"Our SOC2 certification verifies our strong security measures.\"\n  - name: HIPAA\n    claimed: true\n    evidence: Named in the certifications list on the security page.\n  - name: PCI DSS\n    claimed: true\n    evidence: \"SOC2, CCPA, HIPAA, and PCI DSS certifications give you peace of mind.\"\n  - name: GDPR\n    claimed: true\n    type: regulatory compliance (not a certification)\n    evidence: Named in the certifications list on the security page.\n  - name: CCPA\n    claimed: true\n    type: regulatory compliance (not a certification)\n    evidence: >-\n      Named in the certifications list; a dedicated CCPA notice is published at\n      https://signup.liberateinc.com/ccpa\n  - name: ISO 27001\n    claimed: false\n  - name: FedRAMP\n    claimed: false\n\ncontrols_published:\n\
  \  - name: Role and attribute-based access control\n    detail: >-\n      Role-based access controls restrict data access to authorized users; role and attribute-based\n      permissions allow customization within a single role.\n  - name: Project-based permissions\n    detail: Teams can be granted access to specific information within a shared project.\n  - name: Encryption in transit and at rest\n    detail: >-\n      All data, including third-party sourced data, is encrypted. Integration credentials are\n      encrypted both in transit and at rest.\n  - name: Single-tenant data isolation\n    detail: >-\n      \"Unlike typical multi-tenant systems, Liberate never mixes your data with that of other\n      customers.\" Each organization is given its own instance.\n  - name: Audit logging\n    detail: >-\n      Amazon CloudTrail logs and tracks account activity across the AWS infrastructure, providing\n      change attribution and the ability to revert to previous versions.\n  - name:\
  \ Penetration testing\n    detail: Liberate states it regularly conducts penetration tests.\n  - name: Single sign-on\n    detail: SAML SSO brokered through Amazon Cognito. See authentication/liberate-innovations-authentication.yml.\n  - name: Backups\n    detail: Named among data security practices on the security FAQ.\n\ninfrastructure:\n  cloud: AWS\n  region_evidence: >-\n    us-west-2 appears in the documented Cognito ACS URL format\n    (https://<tenant>.auth.us-west-2.amazoncognito.com/saml2/idpresponse).\n  evidence_url: https://docs.liberateinc.com/docs/google-workspace\n\nprivacy:\n  privacy_policy: https://www.liberateinc.com/legal/privacy-policy\n  privacy_policy_effective: '2024-10-15'\n  terms_of_service: https://www.liberateinc.com/legal/terms-of-service\n  ccpa_notice: https://signup.liberateinc.com/ccpa\n  legal_entity: Liberate Innovations, Inc.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberate-innovations/refs/heads/main/security/liberate-innovations-trust-center.yml
summary_line: SOC 2, HIPAA, PCI DSS, GDPR, CCPA, ISO 27001, FedRAMP
tags:
- Company
- Insurance
- InsurTech
- Artificial Intelligence
- Voice AI
- Conversational AI
- Workflow Orchestration
- Claims Automation
- Integration
- Contact Center
trust_url: ''
---
