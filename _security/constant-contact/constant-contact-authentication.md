---
api_key_in:
- header
api_specs:
- filename: constant-contact-account-services-api-openapi.yml
  format: yaml
  label: Constant Contact Account Services API
  slug: constant-contact-account-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-account-services-api-openapi.yml
- filename: constant-contact-bulk-activities-api-openapi.yml
  format: yaml
  label: Constant Contact Bulk Activities API
  slug: constant-contact-bulk-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-bulk-activities-api-openapi.yml
- filename: constant-contact-contact-lists-api-openapi.yml
  format: yaml
  label: Constant Contact Contact Lists API
  slug: constant-contact-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contact-lists-api-openapi.yml
- filename: constant-contact-contact-tags-api-openapi.yml
  format: yaml
  label: Constant Contact Contact Tags API
  slug: constant-contact-contact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contact-tags-api-openapi.yml
- filename: constant-contact-contacts-api-openapi.yml
  format: yaml
  label: Constant Contact Contacts API
  slug: constant-contact-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contacts-api-openapi.yml
- filename: constant-contact-contacts-custom-fields-api-openapi.yml
  format: yaml
  label: Constant Contact Contacts Custom Fields API
  slug: constant-contact-contacts-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contacts-custom-fields-api-openapi.yml
- filename: constant-contact-contacts-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact Contacts Reporting API
  slug: constant-contact-contacts-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-contacts-reporting-api-openapi.yml
- filename: constant-contact-email-campaigns-ab-tests-api-openapi.yml
  format: yaml
  label: Constant Contact Email Campaigns AB Tests API
  slug: constant-contact-email-campaigns-ab-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-campaigns-ab-tests-api-openapi.yml
- filename: constant-contact-email-campaigns-api-openapi.yml
  format: yaml
  label: Constant Contact Email Campaigns API
  slug: constant-contact-email-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-campaigns-api-openapi.yml
- filename: constant-contact-email-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact Email Reporting API
  slug: constant-contact-email-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-reporting-api-openapi.yml
- filename: constant-contact-email-scheduling-api-openapi.yml
  format: yaml
  label: Constant Contact Email Scheduling API
  slug: constant-contact-email-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-email-scheduling-api-openapi.yml
- filename: constant-contact-events-api-openapi.yml
  format: yaml
  label: Constant Contact Events API
  slug: constant-contact-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-events-api-openapi.yml
- filename: constant-contact-landing-pages-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact Landing Pages Reporting API
  slug: constant-contact-landing-pages-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-landing-pages-reporting-api-openapi.yml
- filename: constant-contact-segments-api-openapi.yml
  format: yaml
  label: Constant Contact Segments API
  slug: constant-contact-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-segments-api-openapi.yml
- filename: constant-contact-sms-reporting-api-openapi.yml
  format: yaml
  label: Constant Contact SMS Reporting API
  slug: constant-contact-sms-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-sms-reporting-api-openapi.yml
- filename: constant-contact-technology-partners-api-openapi.yml
  format: yaml
  label: Constant Contact Technology Partners API
  slug: constant-contact-technology-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-technology-partners-api-openapi.yml
- filename: constant-contact-technology-partners-webhooks-api-openapi.yml
  format: yaml
  label: Constant Contact Technology Partners Webhooks API
  slug: constant-contact-technology-partners-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/openapi/constant-contact-technology-partners-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Constant Contact Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Constant Contact secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Constant Contact
provider_slug: constant-contact
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize
    flow: implicit
    scopes: 4
  name: oauth2_implicit
  sources:
  - openapi/constant-contact-v3-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://authz.constantcontact.com/oauth2/default/v1/token
  name: oauth2_access_code
  sources:
  - openapi/constant-contact-v3-openapi.yml
  type: oauth2
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/constant-contact-v3-openapi.yml
  type: apiKey
slug: constant-contact-authentication
source_filename: constant-contact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/constant-contact-v3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: oauth2_implicit\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize\n    scopes: 4\n  sources:\n  - openapi/constant-contact-v3-openapi.yml\n- name: oauth2_access_code\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize\n    tokenUrl: https://authz.constantcontact.com/oauth2/default/v1/token\n    scopes: 4\n  sources:\n  - openapi/constant-contact-v3-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/constant-contact-v3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/authentication/constant-contact-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Campaigns
- Contacts
- Email Marketing
- Events
- Reporting
- SMS
- Surveys
---
