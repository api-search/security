---
api_specs:
- filename: microsoft-power-platform-metadata-api-openapi.yml
  format: yaml
  label: Microsoft Power Platform Metadata API
  slug: microsoft-power-platform-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/microsoft-power-platform-metadata-api-openapi.yml
- filename: microsoft-power-platform-records-api-openapi.yml
  format: yaml
  label: Microsoft Power Platform Records API
  slug: microsoft-power-platform-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/microsoft-power-platform-records-api-openapi.yml
- filename: microsoft-power-platform-enterprise-policies-openapi.json
  format: json
  label: Power Platform Enterprise Policies (Azure Resource Manager)
  slug: microsoft-power-platform-enterprise-policies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/_original/microsoft-power-platform-enterprise-policies-openapi.json
certification_count: 0
certifications: []
description: Microsoft operates a public Trust Center and a Service Trust Portal, and the Power Platform compliance documentation names both as the authoritative source for Power Apps, Power Automate and Power BI trust information.
kind: trust-center
layout: security
name: Microsoft Power Platform Trust Center
name_suffix: Trust Center
overview: Microsoft Power Platform maintains a public trust center covering its security and compliance posture.
provider_name: Microsoft Power Platform
provider_slug: microsoft-power-platform
slug: microsoft-power-platform-trust-center
source_filename: microsoft-power-platform-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.microsoft.com/en-us/trust-center (HTTP 200),\n  https://www.microsoft.com/en-us/trust-center/product-overview (HTTP 200),\n  https://servicetrust.microsoft.com/ (HTTP 200),\n  https://learn.microsoft.com/en-us/power-platform/admin/wp-compliance-data-privacy (HTTP 200)\ndescription: >-\n  Microsoft operates a public Trust Center and a Service Trust Portal, and the Power Platform\n  compliance documentation names both as the authoritative source for Power Apps, Power Automate\n  and Power BI trust information.\ntrust_center:\n  url: https://www.microsoft.com/en-us/trust-center\n  product_overview: https://www.microsoft.com/en-us/trust-center/product-overview\n  status: 200\nservice_trust_portal:\n  url: https://servicetrust.microsoft.com/\n  status: 200\n  gated: true\n  note: >-\n    Audit reports, certificates and attestation documents are downloadable from the Service\n    Trust Portal behind sign-in. Because\
  \ the documents themselves were not retrieved, no\n    individual certification name is asserted in this artifact.\npublished_controls:\n- name: Encryption at rest\n  detail: SQL Server Transparent Data Encryption on every Dataverse database environment.\n- name: Customer-managed encryption keys\n  detail: Self-managed database encryption keys via the Power Platform admin center manage-keys feature.\n  docs: https://learn.microsoft.com/en-us/power-platform/admin/customer-managed-key\n- name: TLS 1.2 or higher\n  detail: Required for all server endpoints; TLSv1.3 observed on probe 2026-09-06.\n- name: Geo-scoped data residency\n  detail: Data stays within the environment's geo except for documented legal and support cases.\n- name: Customer Lockbox\n  detail: >-\n    Exposed as a property (PropertiesLockbox) on the Microsoft.PowerPlatform enterprise policy\n    resource in the ARM contract saved to openapi/_original/.\n- name: Virtual Network injection and Private Link\n  detail: >-\n \
  \   Enterprise policies of kind NetworkInjection plus privateEndpointConnections /\n    privateLinkResources operations in the ARM contract.\n- name: GDPR data subject rights procedures\n  docs: https://learn.microsoft.com/en-us/power-platform/admin/wp-compliance-data-privacy\n- name: US Government cloud (GCC / GCC High)\n  docs: https://learn.microsoft.com/en-us/power-platform/admin/powerapps-us-government\ncertifications_named: []\ncertifications_note: >-\n  Left deliberately empty. The Power Platform compliance page routes to the Trust Center and\n  Service Trust Portal rather than listing certificates, and the Service Trust Portal requires\n  sign-in. Naming ISO/SOC/FedRAMP numbers here without having read the attestation would be a\n  claim this pass did not verify.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/security/microsoft-power-platform-trust-center.yml
summary_line: trust center published
tags:
- Dataverse
- Low-Code
- Microsoft
- Power Apps
- Power Automate
- Power BI
trust_url: ''
---
