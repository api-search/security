---
api_specs:
- filename: constellation-space-openapi.yml
  format: yaml
  label: ConstellationOS API
  slug: constellationos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/openapi/constellation-space-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Constellation Space Trust Center
name_suffix: Trust Center
overview: Constellation Space maintains a public trust center covering its security and compliance posture.
provider_name: Constellation Space
provider_slug: constellation-space
slug: constellation-space-trust-center
source_filename: constellation-space-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: false\nsource: https://constellation.space/security\nurl: https://constellation.space/security\nnote: >-\n  Constellation publishes a security practices page (not a dedicated trust\n  portal). No named third-party certifications (SOC 2, ISO 27001, PCI DSS,\n  HIPAA, FedRAMP) are claimed as of this pass; enterprise customers may request\n  documentation, questionnaires, or security review under NDA.\ncertifications: []\npractices:\n  data_handling: Customer telemetry/topology remain customer data; not sold, not used to train shared models; production tenants isolated.\n  encryption: TLS 1.2+ in transit; encryption at rest for persisted telemetry, credentials, and audit logs.\n  access_control: Role-based access in console and API; automated orchestration runs only under operator-defined policy; admin actions and API calls logged for audit.\n  infrastructure: Hardened cloud infrastructure; separate dev and prod environments; regular\
  \ patch cadence; restricted production access.\n  availability: Platform health and incident history on the status page (https://status.constellation.space/).\nenterprise:\n  deployment: [AWS, Azure, GCP, AWS GovCloud, on-premises / air-gapped]\n  controls: [SSO, RBAC, audit]\n  nda_docs: true\n  contact: contact@constellation.space\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/security/constellation-space-trust-center.yml
summary_line: trust center published
tags:
- Company
- Satellites
- Space
- Telemetry
- Machine Learning
- Fleet Operations
- Ground Segment
- Predictions
trust_url: https://constellation.space/security
---
