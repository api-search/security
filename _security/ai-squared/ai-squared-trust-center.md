---
api_specs:
- filename: ai-squared-catalogs-api-openapi.yml
  format: yaml
  label: AI Squared Catalogs API
  slug: ai-squared-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-catalogs-api-openapi.yml
- filename: ai-squared-connector-definitions-api-openapi.yml
  format: yaml
  label: AI Squared Connector Definitions API
  slug: ai-squared-connector-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-connector-definitions-api-openapi.yml
- filename: ai-squared-connectors-api-openapi.yml
  format: yaml
  label: AI Squared Connectors API
  slug: ai-squared-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-connectors-api-openapi.yml
- filename: ai-squared-models-api-openapi.yml
  format: yaml
  label: AI Squared Models API
  slug: ai-squared-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-models-api-openapi.yml
- filename: ai-squared-syncrecords-api-openapi.yml
  format: yaml
  label: AI Squared Sync Records API
  slug: ai-squared-syncrecords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncrecords-api-openapi.yml
- filename: ai-squared-syncrun-api-openapi.yml
  format: yaml
  label: AI Squared Sync Run API
  slug: ai-squared-syncrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncrun-api-openapi.yml
- filename: ai-squared-syncruns-api-openapi.yml
  format: yaml
  label: AI Squared Sync Runs API
  slug: ai-squared-syncruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncruns-api-openapi.yml
- filename: ai-squared-syncs-api-openapi.yml
  format: yaml
  label: AI Squared Syncs API
  slug: ai-squared-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncs-api-openapi.yml
certification_count: 3
certifications:
- SOC 2 Type II
- HIPAA
- CCPA
description: ''
kind: trust-center
layout: security
name: Ai Squared Trust Center
name_suffix: Trust Center
overview: AI Squared maintains a public trust center documenting SOC 2 Type II, HIPAA, and CCPA compliance.
provider_name: AI Squared
provider_slug: ai-squared
slug: ai-squared-trust-center
source_filename: ai-squared-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  https://docs.squared.ai/deployment-and-security/security-and-compliance/overview and\n  https://aisquared.ai/security-compliance-teams/\ntrust_center:\n  dedicated_portal: false\n  probed:\n  - url: https://trust.squared.ai/\n    result: DNS does not resolve\n  - url: https://trust.aisquared.ai/\n    result: DNS does not resolve\n  - url: https://aisquared.ai/trust/\n    status: 404\n  checked: '2026-09-13'\n  note: >-\n    No Vanta/Drata/SafeBase-style trust portal, and no downloadable report request form. The\n    compliance posture is published as documentation prose and website logos only.\npages:\n- url: https://docs.squared.ai/deployment-and-security/security-and-compliance/overview\n  title: SOC 2 Type II\n  status: 200\n- url: https://aisquared.ai/security-compliance-teams/\n  title: Security & Compliance Teams\n  status: 200\n- url: https://aisquared.ai/data-processing-agreement/\n  title: Data Processing Agreement\n\
  \  status: 200\n- url: https://aisquared.ai/privacy-policy/\n  title: Privacy Policy\n  status: 200\ncertifications:\n- name: SOC 2 Type II\n  claimed: true\n  status: certified\n  evidence: https://docs.squared.ai/deployment-and-security/security-and-compliance/overview\n  quote: >-\n    \"We are SOC 2 Type II certified, demonstrating that we meet stringent standards for\n    information security.\"\n  report_available: not stated\n  auditor: not stated\n  period: not stated\n- name: HIPAA\n  claimed: true\n  status: claimed-badge-only\n  evidence: https://aisquared.ai/security-compliance-teams/\n  note: >-\n    Displayed as a footer badge on the website. No BAA offer, scope statement or attestation\n    detail is published; recorded as a claim, not a verified certification.\n- name: CCPA\n  claimed: true\n  status: claimed-badge-only\n  evidence: https://aisquared.ai/security-compliance-teams/\n  note: Footer badge; a privacy-regime claim rather than a certification.\nnot_claimed:\n\
  - ISO 27001\n- ISO 27701\n- FedRAMP\n- PCI DSS\n- StateRAMP\n- CMMC\n- NIST 800-53\n- GDPR (no explicit claim found, though a DPA is published)\ncontrols_published:\n- control: Encryption at rest and in transit for all customers\n  source: https://docs.squared.ai/deployment-and-security/security-and-compliance/overview\n- control: Encryption key management via Azure Key Vault\n  source: https://docs.squared.ai/deployment-and-security/security-and-compliance/overview\n- control: Customer data isolation / segregation between tenants\n  source: https://docs.squared.ai/deployment-and-security/security-and-compliance/overview\n- control: Hosted on Azure AKS with Azure Key Vault, Azure Defender and Azure Policy\n  source: https://docs.squared.ai/deployment-and-security/security-and-compliance/overview\n- control: Role-Based Access Control restricting staff access to customer data\n  source: https://docs.squared.ai/deployment-and-security/security-and-compliance/overview\n- control: Role-based\
  \ access, encryption and audit logs \"built into every interaction\"; complete\n    audit trails from data source to output\n  source: https://aisquared.ai/security-compliance-teams/\ndeployment_isolation_options:\n- Managed Cloud (SaaS)\n- Customer-Managed Cloud (customer VPC)\n- Air-gapped on-premises\n- Federal on-premises / customer VPC (the Federal tier)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/security/ai-squared-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, CCPA
tags:
- Data Integration
- Reverse ETL
- Artificial Intelligence
- Machine Learning
- Customer Data Platform
- Data Activation
- Workflow Automation
- Open Source
- MCP
- Enterprise
- A2A
trust_url: ''
---
