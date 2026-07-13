---
api_key_in: []
auth_types:
- oauth2
- session
description: ''
kind: authentication
layout: security
method: researched
name: Certinia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Certinia secures its APIs with oauth2 and session across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Certinia
provider_slug: certinia
scheme_count: 3
schemes:
- description: 'Salesforce OAuth 2.0 (web server, JWT bearer, or client credentials flows) issues an access token used as `Authorization: Bearer <token>` against the customer''s Salesforce org (my.salesforce.com domain). Required scopes and the connected app are configured in the customer''s org.'
  name: salesforceOAuth2
  sources:
  - https://help.certinia.com/TechnicalReference/2024.2/RevenueManagement/Apex/GenericAPI.htm
  type: oauth2
- description: Legacy SOAP integrations authenticate with a Salesforce session ID obtained via login(), passed in the SOAP header, for standard SOAP environments (e.g. .NET, Apache Axis).
  in: header
  name: salesforceSession
  sources:
  - https://help.certinia.com/TechnicalReference/2024.2/ProfessionalServicesAutomation/Apex/GenericAPI.htm
  type: apiKey
- description: Beyond authentication, the running user must be granted the Certinia-provided permission set or profile for the relevant managed package before its Apex service classes can be invoked.
  name: permissionSet
  sources:
  - https://help.certinia.com/TechnicalReference/2023.2/Accounting/Apex/GenericAPI.htm
  type: authorization
slug: certinia-authentication
source_filename: certinia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: researched\nsource: Certinia Apex API developer references + Salesforce Platform auth model\nsummary:\n  types:\n  - oauth2\n  - session\n  note: >-\n    Certinia does not operate its own identity provider. Its Apex and legacy SOAP\n    APIs execute inside the customer's Salesforce org, so authentication and\n    authorization are provided entirely by the Salesforce Platform. External\n    integrations authenticate with Salesforce OAuth 2.0 (or a SOAP session ID);\n    in-org Apex-to-Apex calls run in the current user context. Access additionally\n    requires the relevant Certinia managed package to be installed and an\n    appropriate permission set or profile assigned to the running user.\nschemes:\n- name: salesforceOAuth2\n  type: oauth2\n  description: >-\n    Salesforce OAuth 2.0 (web server, JWT bearer, or client credentials flows)\n    issues an access token used as `Authorization: Bearer <token>` against the\n    customer's Salesforce\
  \ org (my.salesforce.com domain). Required scopes and the\n    connected app are configured in the customer's org.\n  sources:\n  - https://help.certinia.com/TechnicalReference/2024.2/RevenueManagement/Apex/GenericAPI.htm\n- name: salesforceSession\n  type: apiKey\n  in: header\n  description: >-\n    Legacy SOAP integrations authenticate with a Salesforce session ID obtained\n    via login(), passed in the SOAP header, for standard SOAP environments\n    (e.g. .NET, Apache Axis).\n  sources:\n  - https://help.certinia.com/TechnicalReference/2024.2/ProfessionalServicesAutomation/Apex/GenericAPI.htm\n- name: permissionSet\n  type: authorization\n  description: >-\n    Beyond authentication, the running user must be granted the Certinia-provided\n    permission set or profile for the relevant managed package before its Apex\n    service classes can be invoked.\n  sources:\n  - https://help.certinia.com/TechnicalReference/2023.2/Accounting/Apex/GenericAPI.htm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certinia/refs/heads/main/authentication/certinia-authentication.yml
summary_line: oauth2/session · 3 schemes
tags:
- Revenue Recognition
- ASC 606
- ERP
- Professional Services Automation
- PSA
- Billing
- Accounting
- Salesforce
- FinancialForce
- Finance
---
