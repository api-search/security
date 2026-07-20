---
api_specs:
- filename: ledge-api-openapi.yml
  format: yaml
  label: Ledge API
  slug: ledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/openapi/ledge-api-openapi.yml
certifications:
- SOC 1
- SOC 2
- ISO 42001
- GDPR
description: Ledge publishes a security overview page at https://www.ledge.co/security that names its compliance attestations and links to a Vanta-hosted trust center at https://trust.ledge.co, where SOC reports, compliance certifications and security policies are made available. The trust center is a client-rendered Vanta application, so its document inventory is not machine-readable from the HTML; the certifications below are quoted from the public security page.
kind: trust-center
layout: security
name: Ledge Trust Center
name_suffix: Trust Center
overview: Ledge maintains a public trust center documenting SOC 1, SOC 2, ISO 42001, and GDPR compliance.
provider_name: Ledge
provider_slug: ledge
slug: ledge-trust-center
source_filename: ledge-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.ledge.co/security\nurl: https://www.ledge.co/security\ntrust_center: https://trust.ledge.co\ntrust_center_platform: Vanta\ndescription: >-\n  Ledge publishes a security overview page at https://www.ledge.co/security that\n  names its compliance attestations and links to a Vanta-hosted trust center at\n  https://trust.ledge.co, where SOC reports, compliance certifications and\n  security policies are made available. The trust center is a client-rendered\n  Vanta application, so its document inventory is not machine-readable from the\n  HTML; the certifications below are quoted from the public security page.\ncertifications:\n- name: SOC 1\n  evidence: Listed on https://www.ledge.co/security\n- name: SOC 2\n  evidence: Listed on https://www.ledge.co/security\n- name: ISO 42001\n  evidence: >-\n    Listed on https://www.ledge.co/security. ISO/IEC 42001 is the AI management\n    system standard, consistent\
  \ with Ledge's AI-agent close-execution product.\n- name: GDPR\n  evidence: Listed on https://www.ledge.co/security\npractices:\n- name: Encryption\n  detail: Encryption in transit and at rest.\n  source: https://www.ledge.co/security\n- name: Penetration testing\n  detail: >-\n    Periodic third-party penetration testing; annual third-party penetration\n    test reports available under NDA.\n  source: https://www.ledge.co/security\n- name: Data processing agreement\n  detail: Standard DPA available for review and execution.\n  source: https://www.ledge.co/security\n- name: SAML 2.0 single sign-on\n  detail: >-\n    Enterprise SSO via any SAML 2.0 IdP (Okta, JumpCloud, Microsoft Entra ID,\n    Google Workspace, OneLogin) against the Auth0-backed auth.goledge.io.\n  source: https://docs.ledge.co/authentication/how-to-guide-configure-saml-sso-with-ledge\n- name: SCIM 2.0 provisioning\n  detail: >-\n    Automated user provisioning and deprovisioning from the IdP via SCIM 2.0\n    with bearer-token\
  \ authentication. Group membership is not synced.\n  source: https://docs.ledge.co/authentication/how-to-guide-configure-scim-provisioning-with-ledge\n- name: Role-based fine-grained permissions\n  detail: >-\n    Built-in Administrator / Full member / View-only roles plus custom roles\n    that allow or deny access to specific resources.\n  source: https://docs.ledge.co/api-reference/fundamentals/fine-grained-permissions\nreports_available:\n- SOC reports (via trust center)\n- Compliance certifications (via trust center)\n- Security policies (via trust center)\n- Annual third-party penetration test report (under NDA)\nnot_found:\n- >-\n  No /.well-known/security.txt on www.ledge.co, api.goledge.io or docs.ledge.co\n  (all 404 at probe time).\n- >-\n  No published vulnerability disclosure policy, responsible-disclosure page or\n  bug bounty program (HackerOne / Bugcrowd / Intigriti) was found.\n- No named ISO 27001, PCI DSS, HIPAA or FedRAMP claim on the public security page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/security/ledge-trust-center.yml
summary_line: SOC 1, SOC 2, ISO 42001, GDPR
tags:
- Company
- Fintech
- Accounting
- Reconciliation
- Financial Close
- Payment Operations
- Transaction Matching
- Cash Application
- Journal Entries
- AI Agents
- ERP Integration
- Finance Automation
trust_url: https://www.ledge.co/security
---
