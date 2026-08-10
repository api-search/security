---
api_specs:
- filename: akuity-apikeyservice-api-openapi.yml
  format: yaml
  label: Akuity API Key Service API
  slug: akuity-apikeyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-apikeyservice-api-openapi.yml
- filename: akuity-argocdservice-api-openapi.yml
  format: yaml
  label: Akuity Argo CD Service API
  slug: akuity-argocdservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-argocdservice-api-openapi.yml
- filename: akuity-authservice-api-openapi.yml
  format: yaml
  label: Akuity Auth Service API
  slug: akuity-authservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-authservice-api-openapi.yml
- filename: akuity-customroleservice-api-openapi.yml
  format: yaml
  label: Akuity Custom Role Service API
  slug: akuity-customroleservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-customroleservice-api-openapi.yml
- filename: akuity-extensionservice-api-openapi.yml
  format: yaml
  label: Akuity Extension Service API
  slug: akuity-extensionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-extensionservice-api-openapi.yml
- filename: akuity-kargoservice-api-openapi.yml
  format: yaml
  label: Akuity Kargo Service API
  slug: akuity-kargoservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-kargoservice-api-openapi.yml
- filename: akuity-organizationservice-api-openapi.yml
  format: yaml
  label: Akuity Organization Service API
  slug: akuity-organizationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-organizationservice-api-openapi.yml
- filename: akuity-systemservice-api-openapi.yml
  format: yaml
  label: Akuity System Service API
  slug: akuity-systemservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/openapi/akuity-systemservice-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2022
- PCI DSS v4.0.1
- HIPAA
- CSA STAR Level 1
- GDPR
description: Akuity operates a Vanta-hosted Trust Center at trust.akuity.io holding audit reports and supporting documentation, and a server-rendered Security and Compliance page at akuity.io/security-compliance that names every framework in plain text. The named certifications below are quoted from that page, which was last updated 2026-01-30 per its own byline.
kind: trust-center
layout: security
name: Akuity Trust Center
name_suffix: Trust Center
overview: Akuity maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001:2022, PCI DSS v4.0.1, HIPAA, CSA STAR Level 1, and GDPR compliance.
provider_name: Akuity
provider_slug: akuity
slug: akuity-trust-center
source_filename: akuity-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://akuity.io/security-compliance + https://trust.akuity.io/\nurl: https://trust.akuity.io/\nprovider: Vanta\ndescription: >-\n  Akuity operates a Vanta-hosted Trust Center at trust.akuity.io holding audit\n  reports and supporting documentation, and a server-rendered Security and\n  Compliance page at akuity.io/security-compliance that names every framework in\n  plain text. The named certifications below are quoted from that page, which was\n  last updated 2026-01-30 per its own byline.\n\ntrust_center:\n  url: https://trust.akuity.io/\n  platform: Vanta\n  machine_readable: false\n  note: >-\n    The trust center is a client-rendered single-page app. It returns HTTP 200\n    with the same HTML shell for every path, including paths that do not exist,\n    so nothing on it is machine-readable and none of its 200s are evidence on\n    their own. The certifications below were therefore read from the\n    server-rendered\
  \ akuity.io/security-compliance page instead.\n  documents_available: audit reports and supporting documentation, on request\n\ncertifications:\n  - name: SOC 2 Type II\n    status: certified\n    scope: Security Trust Service Criteria, operational effectiveness validated over time\n  - name: ISO/IEC 27001:2022\n    status: certified\n    scope: Information Security Management System (ISMS)\n  - name: PCI DSS v4.0.1\n    status: assessed\n    role: Service Provider\n    scope: Report on Compliance (ROC) completed\n    clarification: >-\n      \"Akuity is assessed as a service provider and does not store, process, or\n      transmit cardholder data on behalf of customers.\"\n  - name: HIPAA\n    status: aligned\n    clarification: >-\n      \"Akuity supports HIPAA-regulated workloads through aligned safeguards but\n      is not a covered entity.\"\n  - name: CSA STAR Level 1\n    status: self-assessment\n    clarification: 'Level 1 self-assessment based on publicly available documentation,\
  \ aligned with the Cloud Controls Matrix.'\n  - name: GDPR\n    status: aligned\n    scope: Platform and operational practices designed to support GDPR data-protection principles\n\ndata_residency:\n  - region: United States\n    detail: Deployed across multiple availability zones.\n  - region: European Union\n    detail: >-\n      Fully self-contained EU region. Primary in Frankfurt, Germany with a\n      secondary backup region in Ireland. Customer data, including logs and\n      telemetry, remains within the EU.\n\nencryption:\n  in_transit: TLS 1.2 or higher\n  at_rest: AES-256 for databases, object storage and backups\n  key_management: AWS KMS, separation of duties, no shared or hard-coded keys\n  byok: https://docs.akuity.io/akuity-portal/security/byok\n\ndata_handling:\n  sells_customer_data: false\n  uses_customer_data_for_advertising: false\n  trains_ai_on_customer_data: false\n  ai_clarification: >-\n    \"Akuity does not use customer data to train machine learning or AI models\n\
  \    without explicit customer consent.\" Akuity Intelligence uses live platform\n    context (logs, events, manifests, deployment history) at inference time.\n  support_access: limited, approved, time-bound, logged, revoked on completion\n  deletion: >-\n    Documented retention and deletion policies; customer data securely deleted\n    within defined timeframes on termination or request, with confirmation of\n    deletion available on request.\n\noperational_controls:\n  secure_sdlc:\n    - Mandatory peer review for all code changes\n    - Version-controlled change management\n    - Automated testing and security checks in CI/CD\n    - Dependency scanning and vulnerability detection\n    - Separation of duties between development and production access\n  monitoring:\n    - Centralized logging across infrastructure and applications\n    - Audit logging for administrative and access activities\n    - Continuous monitoring for anomalous behaviour\n  business_continuity:\n    - Continuous\
  \ backups of customer data\n    - Backups stored in a secondary region\n    - Documented and regularly tested disaster recovery procedures\n  employee_security:\n    - Background checks prior to access\n    - Mandatory security and privacy training\n    - Additional secure coding training for engineers\n  third_party_risk:\n    - Risk-based vendor assessment\n    - Review of third-party security attestations\n    - Least-privilege vendor access\n\ninfrastructure:\n  cloud: Amazon Web Services\n  network:\n    - WAF and DDoS protection\n    - Strictly controlled network access\n    - Segmented networks and access boundaries\n    - Logical isolation between customer environments\n  private_link: https://docs.akuity.io/akuity-portal/security/private-link\n  networking_requirements: https://docs.akuity.io/akuity-portal/security/akp-networking-requirements\n\nsecurity_contact: security@akuity.io\nsee_also:\n  - security/akuity-vulnerability-disclosure.yml\n  - security/akuity-domain-security.yml\n\
  \  - conformance/akuity-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akuity/refs/heads/main/security/akuity-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2022, PCI DSS v4.0.1, HIPAA, CSA STAR Level 1, GDPR
tags:
- GitOps
- Continuous Delivery
- Kubernetes
- Argo CD
- Kargo
- Platform Engineering
- DevOps
- Progressive Delivery
- Cloud Native
- AIOps
- Developer Tools
trust_url: https://trust.akuity.io/
---
