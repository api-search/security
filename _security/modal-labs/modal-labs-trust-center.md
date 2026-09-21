---
api_specs:
- filename: modal-labs-modal-web-endpoints-representative-api-openapi.yml
  format: yaml
  label: Modal Web Endpoints (Representative) API
  slug: modal-labs-modal-web-endpoints-representative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-labs/refs/heads/main/openapi/modal-labs-modal-web-endpoints-representative-api-openapi.yml
certification_count: 3
certifications:
- SOC 2 Type 2
- HIPAA
- PCI DSS
description: Modal runs a Vanta-hosted security portal at trust.modal.com where the SOC 2 Type 2 report is requested under NDA, and documents its compliance posture in the public docs. The portal itself is a client-rendered SPA — every certification recorded here is read from Modal's own first-party documentation, not scraped from the portal.
kind: trust-center
layout: security
name: Modal Labs Trust Center
name_suffix: Trust Center
overview: Modal maintains a public trust center documenting SOC 2 Type 2, HIPAA, and PCI DSS compliance.
provider_name: Modal
provider_slug: modal-labs
slug: modal-labs-trust-center
source_filename: modal-labs-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://modal.com/docs/guide/security + https://trust.modal.com/\nprovider: Modal\nproviderId: modal-labs\ndescription: >-\n  Modal runs a Vanta-hosted security portal at trust.modal.com where the SOC 2\n  Type 2 report is requested under NDA, and documents its compliance posture in\n  the public docs. The portal itself is a client-rendered SPA — every\n  certification recorded here is read from Modal's own first-party\n  documentation, not scraped from the portal.\nurl: https://trust.modal.com/\nplatform: Vanta\nplatform_evidence: >-\n  content-location header resolves to\n  assets.vanta.com/static/index-trust-report.<hash>.html; probed 2026-09-18, HTTP 200.\naccess: >-\n  Report access is gated — \"Go to our Security Portal to request access to the\n  report.\"\ncertifications:\n- name: SOC 2 Type 2\n  status: achieved\n  evidence: >-\n    \"We have successfully completed a System and Organization Controls (SOC) 2\n    Type\
  \ 2 audit.\"\n  report_url: https://trust.modal.com/\n  announcement: https://modal.com/blog/soc2type2\n  public_report: false\n- name: HIPAA\n  status: supported-via-BAA\n  evidence: >-\n    \"Modal's services can be used in a HIPAA compliant manner... To use Modal\n    services for HIPAA-compliant workloads, a Business Associate Agreement (BAA)\n    should be established with us prior to submission of any PHI. This is\n    available on our Enterprise plan.\"\n  note: >-\n    Modal is explicit that there is no official HIPAA certification and that\n    scope is partial: Volumes v1, Images (excluding Filesystem and Directory\n    Snapshots), Memory Snapshots and user code are OUT of BAA scope. Volumes v2\n    are in scope.\n  url: https://modal.com/docs/guide/security\n- name: PCI DSS\n  status: not-applicable\n  evidence: >-\n    Modal does not store or process credit card information; card handling is\n    delegated to Stripe, which is certified as a PCI Level 1 Service Provider.\n \
  \ url: https://modal.com/docs/guide/security\nprograms:\n- name: Audit logs\n  url: https://modal.com/docs/guide/audit-logs\n  note: Workspace audit logs, Enterprise plan.\n- name: Data residency\n  url: https://modal.com/docs/guide/data-residency\n- name: Customer-supplied encryption keys\n  url: https://modal.com/docs/guide/customer-supplied-encryption-keys\n  status: Alpha\n- name: Role-Based Access Control\n  url: https://modal.com/docs/guide/rbac\n- name: SSO\n  url: https://modal.com/docs/guide/okta-sso\n  note: Okta, Microsoft Entra and custom SAML SSO are documented separately.\ndata_handling:\n  zero_data_retention_surface: >-\n    Modal Inference endpoints are documented as zero data retention — request and\n    response payloads are never written to disk.\n  function_io_retention: Up to 7 days, encrypted at rest, then deleted.\n  log_retention: 1 day (Starter), 30 days (Team), configurable (Enterprise).\n  commitment: >-\n    \"Modal will never access or use: your source code;\
  \ the inputs or outputs to\n    your Modal Functions; any data you store in Modal, such as in Images or\n    Volumes.\"\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modal-labs/refs/heads/main/security/modal-labs-trust-center.yml
summary_line: SOC 2 Type 2, HIPAA, PCI DSS
tags:
- Serverless
- Compute
- GPU
- AI Infrastructure
- Sandbox
- Infrastructure as Code
trust_url: https://trust.modal.com/
---
