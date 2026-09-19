---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-cost-management-exports-api-openapi.yml
  format: yaml
  label: Azure Cost Management Exports API
  slug: microsoft-azure-cost-management-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-exports-api-openapi.yml
- filename: microsoft-azure-cost-management-operations-api-openapi.yml
  format: yaml
  label: Azure Cost Management Operations API
  slug: microsoft-azure-cost-management-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-operations-api-openapi.yml
- filename: microsoft-azure-cost-management-alerts-api-openapi.yml
  format: yaml
  label: Azure Cost Management Alerts API
  slug: microsoft-azure-cost-management-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-alerts-api-openapi.yml
- filename: microsoft-azure-cost-management-budgets-api-openapi.yml
  format: yaml
  label: Azure Cost Management Budgets API
  slug: microsoft-azure-cost-management-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-budgets-api-openapi.yml
- filename: microsoft-azure-cost-management-costallocationruledefinitions-api-openapi.yml
  format: yaml
  label: Azure Cost Management Cost Allocation Rule Definitions API
  slug: microsoft-azure-cost-management-costallocationruledefinitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-costallocationruledefinitions-api-openapi.yml
- filename: microsoft-azure-cost-management-generatecostdetailsreport-api-openapi.yml
  format: yaml
  label: Azure Cost Management Generate Cost Details Report API
  slug: microsoft-azure-cost-management-generatecostdetailsreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-generatecostdetailsreport-api-openapi.yml
- filename: microsoft-azure-cost-management-generatedetailedcostreportoperationresults-api-openapi.yml
  format: yaml
  label: Azure Cost Management Generate Detailed Cost Report Operation Results API
  slug: microsoft-azure-cost-management-generatedetailedcostreportoperationresults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationresults-api-openapi.yml
- filename: microsoft-azure-cost-management-generatedetailedcostreportoperationstatus-api-openapi.yml
  format: yaml
  label: Azure Cost Management Generate Detailed Cost Report Operation Status API
  slug: microsoft-azure-cost-management-generatedetailedcostreportoperationstatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationstatus-api-openapi.yml
- filename: microsoft-azure-cost-management-markuprules-api-openapi.yml
  format: yaml
  label: Azure Cost Management Markup Rules API
  slug: microsoft-azure-cost-management-markuprules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-markuprules-api-openapi.yml
- filename: microsoft-azure-cost-management-providers-api-openapi.yml
  format: yaml
  label: Azure Cost Management Providers API
  slug: microsoft-azure-cost-management-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-providers-api-openapi.yml
- filename: microsoft-azure-cost-management-scheduledactionoperationgroup-api-openapi.yml
  format: yaml
  label: Azure Cost Management Scheduled Action Operation Group API
  slug: microsoft-azure-cost-management-scheduledactionoperationgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-scheduledactionoperationgroup-api-openapi.yml
- filename: microsoft-azure-cost-management-scheduledactions-api-openapi.yml
  format: yaml
  label: Azure Cost Management Scheduled Actions API
  slug: microsoft-azure-cost-management-scheduledactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-scheduledactions-api-openapi.yml
- filename: microsoft-azure-cost-management-settings-api-openapi.yml
  format: yaml
  label: Azure Cost Management Settings API
  slug: microsoft-azure-cost-management-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-settings-api-openapi.yml
- filename: microsoft-azure-cost-management-viewoperationgroup-api-openapi.yml
  format: yaml
  label: Azure Cost Management View Operation Group API
  slug: microsoft-azure-cost-management-viewoperationgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-viewoperationgroup-api-openapi.yml
- filename: microsoft-azure-cost-management-views-api-openapi.yml
  format: yaml
  label: Azure Cost Management Views API
  slug: microsoft-azure-cost-management-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/openapi/microsoft-azure-cost-management-views-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Microsoft Azure Cost Management Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Cost Management secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Cost Management
provider_slug: microsoft-azure-cost-management
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-cost-management-alerts-api-openapi.yml
  - openapi/microsoft-azure-cost-management-budgets-api-openapi.yml
  - openapi/microsoft-azure-cost-management-costallocationruledefinitions-api-openapi.yml
  - openapi/microsoft-azure-cost-management-exports-api-openapi.yml
  - openapi/microsoft-azure-cost-management-generatecostdetailsreport-api-openapi.yml
  - openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationresults-api-openapi.yml
  - openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationstatus-api-openapi.yml
  - openapi/microsoft-azure-cost-management-markuprules-api-openapi.yml
  - openapi/microsoft-azure-cost-management-operations-api-openapi.yml
  - openapi/microsoft-azure-cost-management-providers-api-openapi.yml
  - openapi/microsoft-azure-cost-management-scheduledactionoperationgroup-api-openapi.yml
  - openapi/microsoft-azure-cost-management-scheduledactions-api-openapi.yml
  - openapi/microsoft-azure-cost-management-settings-api-openapi.yml
  - openapi/microsoft-azure-cost-management-viewoperationgroup-api-openapi.yml
  - openapi/microsoft-azure-cost-management-views-api-openapi.yml
  type: oauth2
slug: microsoft-azure-cost-management-authentication
source_filename: microsoft-azure-cost-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/microsoft-azure-cost-management-alerts-api-openapi.yml, openapi/microsoft-azure-cost-management-budgets-api-openapi.yml,\n  openapi/microsoft-azure-cost-management-costallocationruledefinitions-api-openapi.yml, openapi/microsoft-azure-cost-management-exports-api-openapi.yml,\n  openapi/microsoft-azure-cost-management-generatecostdetailsreport-api-openapi.yml, openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationresults-api-openapi.yml,\n  openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationstatus-api-openapi.yml,\n  openapi/microsoft-azure-cost-management-markuprules-api-openapi.yml, openapi/microsoft-azure-cost-management-operations-api-openapi.yml,\n  openapi/microsoft-azure-cost-management-providers-api-openapi.yml, openapi/microsoft-azure-cost-management-scheduledactionoperationgroup-api-openapi.yml,\n  openapi/microsoft-azure-cost-management-scheduledactions-api-openapi.yml\
  \ ...\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-cost-management-alerts-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-budgets-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-costallocationruledefinitions-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-exports-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-generatecostdetailsreport-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationresults-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-generatedetailedcostreportoperationstatus-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-markuprules-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-operations-api-openapi.yml\n\
  \  - openapi/microsoft-azure-cost-management-providers-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-scheduledactionoperationgroup-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-scheduledactions-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-settings-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-viewoperationgroup-api-openapi.yml\n  - openapi/microsoft-azure-cost-management-views-api-openapi.yml\ndocs:\n- https://learn.microsoft.com/en-us/rest/api/azure/\n- https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth2-client-creds-grant-flow\n- https://learn.microsoft.com/en-us/azure/cost-management-billing/costs/assign-access-acm-data\n- https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles/management-and-governance\ndiscovery: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\ndiscovery_artifact: well-known/microsoft-azure-cost-management-openid-configuration.json\n\
  provider: Microsoft Entra ID\nresource: https://management.azure.com\ntoken_header: 'Authorization: Bearer <token>'\ndocs_note: >-\n  The contract declares one securityScheme, azure_auth, with the implicit flow and the single\n  delegated scope user_impersonation. That is the Azure Resource Manager boilerplate every ARM\n  swagger carries; it is not how a service principal or an agent actually authenticates. Microsoft\n  Entra ID also issues client-credentials tokens for the resource https://management.azure.com\n  (scope https://management.azure.com/.default), which is the unattended path, and\n  authorization-code tokens for delegated user access. The OpenID Provider metadata was fetched\n  and saved; the implicit flow the swagger names is not the only option and should not be read as\n  a constraint.\nauthorization_model:\n  style: azure-rbac\n  note: >-\n    Cost Management does not authorize by OAuth scope. Once a token is accepted, what it can see\n    and change is decided by Azure\
  \ RBAC role assignments at the {scope} in the request path.\n  roles:\n  - name: Cost Management Reader\n    grants: read cost data, budgets, views, alerts and exports at the assigned scope\n  - name: Cost Management Contributor\n    grants: read plus create, update and delete budgets, exports, views and scheduled actions\n  source: https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles/management-and-governance\nscope_paths:\n  note: >-\n    Billing-account and billing-profile scopes use billing-account roles (Enterprise Agreement\n    enrollment roles, or Microsoft Customer Agreement billing roles) rather than Azure RBAC.\n  source: https://learn.microsoft.com/en-us/azure/cost-management-billing/costs/understand-work-scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cost-management/refs/heads/main/authentication/microsoft-azure-cost-management-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cost Management
- FinOps
- Cloud Cost
- Billing
- Budgets
- Export
- Cost Analysis
- Forecasting
- Chargebacks
- Focus
- Azure
- Reservations
---
