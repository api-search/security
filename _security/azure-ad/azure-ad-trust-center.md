---
api_specs:
- filename: azure-ad-graph-applications-openapi.yml
  format: yaml
  label: Azure Active Directory Applications API
  slug: azure-ad-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-applications-openapi.yml
- filename: azure-ad-graph-identity-directorymanagement-openapi.yml
  format: yaml
  label: Azure Active Directory Directory API
  slug: azure-ad-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-directorymanagement-openapi.yml
- filename: azure-ad-graph-groups-openapi.yml
  format: yaml
  label: Azure Active Directory Groups API
  slug: azure-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-groups-openapi.yml
- filename: azure-ad-me-api-openapi.yml
  format: yaml
  label: Azure Active Directory Me API
  slug: azure-ad-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/azure-ad-me-api-openapi.yml
- filename: azure-ad-graph-users-openapi.yml
  format: yaml
  label: Azure Active Directory Users API
  slug: azure-ad-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-users-openapi.yml
- filename: azure-ad-graph-identity-signins-openapi.yml
  format: yaml
  label: Microsoft Entra ID Sign-Ins and Policies API
  slug: azure-ad-signins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-signins-openapi.yml
- filename: azure-ad-graph-identity-governance-openapi.yml
  format: yaml
  label: Microsoft Entra ID Governance API
  slug: azure-ad-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-governance-openapi.yml
- filename: azure-ad-graph-directoryobjects-openapi.yml
  format: yaml
  label: Microsoft Entra ID Directory Objects API
  slug: azure-ad-directory-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-directoryobjects-openapi.yml
- filename: azure-ad-graph-changenotifications-openapi.yml
  format: yaml
  label: Microsoft Entra ID Change Notifications API
  slug: azure-ad-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-changenotifications-openapi.yml
certification_count: 4
certifications:
- FedRAMP
- NIST SP 800-53
- HIPAA / HITECH
- SOX
description: ''
kind: trust-center
layout: security
name: Azure Ad Trust Center
name_suffix: Trust Center
overview: Microsoft Entra ID (formerly Azure AD) maintains a public trust center documenting FedRAMP, NIST SP 800-53, HIPAA / HITECH, and SOX compliance.
provider_name: Microsoft Entra ID (formerly Azure AD)
provider_slug: azure-ad
slug: azure-ad-trust-center
source_filename: azure-ad-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.microsoft.com/en-us/trust-center (probed 200),\n  https://servicetrust.microsoft.com/ (probed 200),\n  https://learn.microsoft.com/en-us/entra/standards/standards-overview,\n  https://learn.microsoft.com/en-us/azure/compliance/\nprovider: Azure Active Directory (Microsoft Entra ID)\nproviderId: azure-ad\ntrust_center:\n  url: https://www.microsoft.com/en-us/trust-center\n  http_status: 200\n  probed: '2026-09-06'\naudit_portal:\n  name: Microsoft Service Trust Portal\n  url: https://servicetrust.microsoft.com/\n  http_status: 200\n  probed: '2026-09-06'\n  note: >-\n    Where the actual audit reports (SOC 1/2/3, ISO certificates, FedRAMP\n    packages, penetration-test summaries) are downloaded. Access to the reports\n    requires sign-in with a Microsoft account; the portal itself is public.\ncompliance_catalog:\n  url: https://learn.microsoft.com/en-us/azure/compliance/offerings/\n  claim: >-\n    \"There\
  \ are 90 Azure compliance certifications ... Azure has 35 compliance\n    offerings for key industries\" — quoted from\n    https://learn.microsoft.com/en-us/entra/standards/standards-overview\n  industries_named:\n    - Health\n    - Government\n    - Finance\n    - Education\n    - Manufacturing\n    - Media\ncertifications:\n  - name: FedRAMP\n    scope: US Federal Risk and Authorization Management Program\n    evidence: https://learn.microsoft.com/en-us/azure/compliance/offerings/offering-fedramp\n  - name: NIST SP 800-53\n    scope: US federal information systems control catalog\n    evidence: https://learn.microsoft.com/en-us/azure/compliance/offerings/offering-nist-800-53\n  - name: HIPAA / HITECH\n    scope: US healthcare\n    evidence: https://learn.microsoft.com/en-us/azure/compliance/offerings/offering-hipaa-us\n  - name: SOX\n    scope: Sarbanes-Oxley Act of 2002\n    evidence: https://learn.microsoft.com/en-us/compliance/regulatory/offering-sox\ncertifications_note: >-\n \
  \ Only the frameworks Microsoft's own Entra standards page names directly are\n  listed above with evidence URLs. Microsoft's wider catalogue (ISO/IEC 27001,\n  27017, 27018, 27701, SOC 1/2/3, PCI DSS, CSA STAR and the rest of the 90) is\n  published per-offering under\n  https://learn.microsoft.com/en-us/azure/compliance/offerings/ and is\n  downloadable from the Service Trust Portal; it is not restated here because it\n  was not read item by item during this pass.\nshared_responsibility:\n  note: >-\n    Microsoft states plainly that compliance is shared: Azure certification is a\n    starting point, and the customer must still configure Microsoft Entra ID to\n    meet the identity standard they are held to. Entra publishes per-standard\n    configuration guidance (for example NIST authenticator assurance levels and\n    FedRAMP High) under https://learn.microsoft.com/en-us/entra/standards/.\nprivacy:\n  privacy_statement: https://www.microsoft.com/en-us/privacy/privacystatement\n  gdpr:\
  \ https://learn.microsoft.com/en-us/compliance/regulatory/gdpr\n  data_residency: https://learn.microsoft.com/en-us/entra/identity/data-residency-and-customer-data\nsovereign_clouds:\n  - name: Microsoft Azure Government (US Gov L4 / L5 DoD)\n  - name: Microsoft Azure operated by 21Vianet (China)\nsovereign_clouds_note: >-\n  Relevant to agent surfaces: the Microsoft MCP Server for Enterprise is global\n    service only and is NOT available in US Gov L4, US Gov L5 (DOD) or 21Vianet —\n    see mcp/azure-ad-mcp.yml availability.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/security/azure-ad-trust-center.yml
summary_line: FedRAMP, NIST SP 800-53, HIPAA / HITECH, SOX
tags:
- Authentication
- Authorization
- Identity
- OpenID Connect
- Single Sign-On
trust_url: ''
---
