---
api_key_in:
- header
api_specs:
- filename: moengage-data-openapi.yml
  format: yaml
  label: MoEngage Data API
  slug: moengage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-data-openapi.yml
- filename: moengage-campaign-draft-openapi.yml
  format: yaml
  label: MoEngage Campaigns API
  slug: moengage-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-campaign-draft-openapi.yml
- filename: moengage-push-openapi.yml
  format: yaml
  label: MoEngage Push API
  slug: moengage-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-push-openapi.yml
- filename: moengage-custom-segments-openapi.yml
  format: yaml
  label: MoEngage Segments API
  slug: moengage-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-custom-segments-openapi.yml
- filename: moengage-email-templates-1-openapi.yml
  format: yaml
  label: MoEngage Content and Templates API
  slug: moengage-content-and-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-email-templates-1-openapi.yml
- filename: moengage-catalog-openapi.yml
  format: yaml
  label: MoEngage Catalog, Recommendations and Coupons API
  slug: moengage-catalog-recommendations-and-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-catalog-openapi.yml
- filename: moengage-email-subscription-openapi.yml
  format: yaml
  label: MoEngage Subscriptions API
  slug: moengage-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-email-subscription-openapi.yml
- filename: moengage-analytics-openapi.yml
  format: yaml
  label: MoEngage Analytics and Flows API
  slug: moengage-analytics-and-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-analytics-openapi.yml
- filename: moengage-inform-openapi.yml
  format: yaml
  label: MoEngage Inform API
  slug: moengage-inform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-inform-openapi.yml
- filename: moengage-cards-openapi.yml
  format: yaml
  label: MoEngage Engagement Surfaces API
  slug: moengage-engagement-surfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-cards-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moengage Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoEngage secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MoEngage
provider_slug: moengage
scheme_count: 3
schemes:
- description: 'Authentication is done via Basic Auth. This requires a base64-encoded string of your credentials in the format `username:password`.


    - **Username**: Use your MoEngage workspace ID (also known as the App ID). You can find it in the MoEngage dashboard at **Settings** > **Account** > **APIs** > **Workspace ID (earlier app id)**.

    - **Password**: Use your Data API Key, which you can find in the MoEngag'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/moengage-analytics-openapi.yml
  - openapi/moengage-business-events-openapi.yml
  - openapi/moengage-campaign-draft-openapi.yml
  - openapi/moengage-campaigns-openapi.yml
  - openapi/moengage-cards-openapi.yml
  - openapi/moengage-catalog-openapi.yml
  - openapi/moengage-cohort-audience-openapi.yml
  - openapi/moengage-content-blocks-openapi.yml
  - openapi/moengage-coupons-openapi.yml
  - openapi/moengage-custom-segments-openapi.yml
  - openapi/moengage-data-openapi.yml
  - openapi/moengage-email-subscription-openapi.yml
  - openapi/moengage-email-templates-1-openapi.yml
  - openapi/moengage-email-templates-2-openapi.yml
  - openapi/moengage-flows-openapi.yml
  - openapi/moengage-gdpr-ccpa-openapi.yml
  - openapi/moengage-in-app-templates-openapi.yml
  - openapi/moengage-inform-openapi.yml
  - openapi/moengage-live-activities-openapi.yml
  - openapi/moengage-message-archival-openapi.yml
  - openapi/moengage-offerings-openapi.yml
  - openapi/moengage-osm-templates-openapi.yml
  - openapi/moengage-personalize-experience-openapi.yml
  - openapi/moengage-push-openapi.yml
  - openapi/moengage-push-templates-openapi.yml
  - openapi/moengage-push-v2-1-openapi.yml
  - openapi/moengage-recommendations-openapi.yml
  - openapi/moengage-sms-templates-openapi.yml
  - openapi/moengage-stats-report-openapi.yml
  - openapi/moengage-subscription-categories-openapi.yml
  type: http
- description: This is the Workspace ID of your MoEngage account that must be passed with the request. You can find it in the MoEngage dashboard at **Settings** > **Account** > **APIs** > **Workspace ID (earlier app id)**.
  in: header
  name: AppKeyHeader
  parameter: MOE-APPKEY
  sources:
  - openapi/moengage-catalog-openapi.yml
  - openapi/moengage-inform-openapi.yml
  - openapi/moengage-push-openapi.yml
  - openapi/moengage-push-v2-1-openapi.yml
  type: apiKey
- description: Custom SHA256 Signature. Refer [here](/api/campaign-reports/download-campaign-report#generating-the-signature).
  in: header
  name: apiKeySignature
  parameter: Signature
  sources:
  - openapi/moengage-stats-report-openapi.yml
  type: apiKey
slug: moengage-authentication
source_filename: moengage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/moengage-analytics-openapi.yml, openapi/moengage-business-events-openapi.yml,\n  openapi/moengage-campaign-draft-openapi.yml, openapi/moengage-campaigns-openapi.yml, openapi/moengage-cards-openapi.yml,\n  openapi/moengage-catalog-openapi.yml, openapi/moengage-cohort-audience-openapi.yml, openapi/moengage-content-blocks-openapi.yml,\n  openapi/moengage-coupons-openapi.yml, openapi/moengage-custom-segments-openapi.yml, openapi/moengage-data-openapi.yml,\n  openapi/moengage-email-subscription-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Authentication is done via Basic Auth. This requires a base64-encoded string of your credentials in the format `username:password`.\n\n    - **Username**: Use your MoEngage workspace ID (also known as the App ID). You can find it in the MoEngage dashboard at **Settings**\
  \ > **Account** > **APIs** > **Workspace ID (earlier app id)**.\n    - **Password**: Use your Data API Key, which you can find in the MoEngag\n  sources:\n  - openapi/moengage-analytics-openapi.yml\n  - openapi/moengage-business-events-openapi.yml\n  - openapi/moengage-campaign-draft-openapi.yml\n  - openapi/moengage-campaigns-openapi.yml\n  - openapi/moengage-cards-openapi.yml\n  - openapi/moengage-catalog-openapi.yml\n  - openapi/moengage-cohort-audience-openapi.yml\n  - openapi/moengage-content-blocks-openapi.yml\n  - openapi/moengage-coupons-openapi.yml\n  - openapi/moengage-custom-segments-openapi.yml\n  - openapi/moengage-data-openapi.yml\n  - openapi/moengage-email-subscription-openapi.yml\n  - openapi/moengage-email-templates-1-openapi.yml\n  - openapi/moengage-email-templates-2-openapi.yml\n  - openapi/moengage-flows-openapi.yml\n  - openapi/moengage-gdpr-ccpa-openapi.yml\n  - openapi/moengage-in-app-templates-openapi.yml\n  - openapi/moengage-inform-openapi.yml\n  - openapi/moengage-live-activities-openapi.yml\n\
  \  - openapi/moengage-message-archival-openapi.yml\n  - openapi/moengage-offerings-openapi.yml\n  - openapi/moengage-osm-templates-openapi.yml\n  - openapi/moengage-personalize-experience-openapi.yml\n  - openapi/moengage-push-openapi.yml\n  - openapi/moengage-push-templates-openapi.yml\n  - openapi/moengage-push-v2-1-openapi.yml\n  - openapi/moengage-recommendations-openapi.yml\n  - openapi/moengage-sms-templates-openapi.yml\n  - openapi/moengage-stats-report-openapi.yml\n  - openapi/moengage-subscription-categories-openapi.yml\n- name: AppKeyHeader\n  type: apiKey\n  in: header\n  parameter: MOE-APPKEY\n  description: This is the Workspace ID of your MoEngage account that must be passed with the\n    request. You can find it in the MoEngage dashboard at **Settings** > **Account** > **APIs**\n    > **Workspace ID (earlier app id)**.\n  sources:\n  - openapi/moengage-catalog-openapi.yml\n  - openapi/moengage-inform-openapi.yml\n  - openapi/moengage-push-openapi.yml\n  - openapi/moengage-push-v2-1-openapi.yml\n\
  - name: apiKeySignature\n  type: apiKey\n  in: header\n  parameter: Signature\n  description: Custom SHA256 Signature. Refer [here](/api/campaign-reports/download-campaign-report#generating-the-signature).\n  sources:\n  - openapi/moengage-stats-report-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/authentication/moengage-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- customer-engagement
- marketing-automation
- customer-data-platform
- push-notifications
- email
- sms
- whatsapp
- in-app-messaging
- segmentation
- personalization
- campaign-management
- analytics
- mobile-sdk
- mcp
- martech
---
