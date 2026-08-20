---
api_key_in: []
api_specs:
- filename: dotdigital-v2-api-full-openapi.yml
  format: yaml
  label: Dotdigital v2 API
  slug: dotdigital-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/openapi/dotdigital-v2-api-full-openapi.yml
- filename: dotdigital-contacts-openapi.yml
  format: yaml
  label: Dotdigital v3 API
  slug: dotdigital-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/openapi/dotdigital-contacts-openapi.yml
- filename: dotdigital-omnichannel-openapi.yml
  format: yaml
  label: Dotdigital CPaaS API
  slug: dotdigital-cpaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/openapi/dotdigital-omnichannel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dotdigital Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dotdigital secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dotdigital
provider_slug: dotdigital
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/dotdigital-accounts-and-utilities-openapi.yml
  - openapi/dotdigital-analytics-openapi.yml
  - openapi/dotdigital-campaign-templates-openapi.yml
  - openapi/dotdigital-chat-config-openapi.yml
  - openapi/dotdigital-chat-message-openapi.yml
  - openapi/dotdigital-chat-openapi.yml
  - openapi/dotdigital-chat-presence-openapi.yml
  - openapi/dotdigital-configuration-service-openapi.yml
  - openapi/dotdigital-contact-data-fields-openapi.yml
  - openapi/dotdigital-contacts-openapi.yml
  - openapi/dotdigital-content-openapi.yml
  - openapi/dotdigital-conversation-message-openapi.yml
  - openapi/dotdigital-conversation-openapi.yml
  - openapi/dotdigital-cpaas-openapi.yml
  - openapi/dotdigital-data-firehose-openapi.yml
  - openapi/dotdigital-documents-openapi.yml
  - openapi/dotdigital-ecommerce-openapi.yml
  - openapi/dotdigital-email-campaigns-openapi.yml
  - openapi/dotdigital-email-contacts-openapi.yml
  - openapi/dotdigital-events-openapi.yml
  - openapi/dotdigital-images-openapi.yml
  - openapi/dotdigital-insight-and-transactional-data-openapi.yml
  - openapi/dotdigital-insight-data-service-openapi.yml
  - openapi/dotdigital-lists-address-books-openapi.yml
  - openapi/dotdigital-marketing-email-openapi.yml
  - openapi/dotdigital-message-history-openapi.yml
  - openapi/dotdigital-message-rules-openapi.yml
  - openapi/dotdigital-omnichannel-openapi.yml
  - openapi/dotdigital-pages-and-forms-openapi.yml
  - openapi/dotdigital-phone-number-validation-openapi.yml
  - openapi/dotdigital-preferences-and-subscriptions-openapi.yml
  - openapi/dotdigital-product-recommendations-openapi.yml
  - openapi/dotdigital-profile-openapi.yml
  - openapi/dotdigital-programs-openapi.yml
  - openapi/dotdigital-scoring-openapi.yml
  - openapi/dotdigital-segments-openapi.yml
  - openapi/dotdigital-session-openapi.yml
  - openapi/dotdigital-sms-campaigns-openapi.yml
  - openapi/dotdigital-templates-openapi.yml
  - openapi/dotdigital-transactional-email-openapi.yml
  - openapi/dotdigital-webhook-openapi.yml
  - openapi/dotdigital-whatsapp-channel-openapi.yml
  type: http
slug: dotdigital-authentication
source_filename: dotdigital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/dotdigital-accounts-and-utilities-openapi.yml, openapi/dotdigital-analytics-openapi.yml,\n  openapi/dotdigital-campaign-templates-openapi.yml, openapi/dotdigital-chat-config-openapi.yml,\n  openapi/dotdigital-chat-message-openapi.yml, openapi/dotdigital-chat-openapi.yml, openapi/dotdigital-chat-presence-openapi.yml,\n  openapi/dotdigital-configuration-service-openapi.yml, openapi/dotdigital-contact-data-fields-openapi.yml,\n  openapi/dotdigital-contacts-openapi.yml, openapi/dotdigital-content-openapi.yml, openapi/dotdigital-conversation-message-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/dotdigital-accounts-and-utilities-openapi.yml\n  - openapi/dotdigital-analytics-openapi.yml\n  - openapi/dotdigital-campaign-templates-openapi.yml\n  - openapi/dotdigital-chat-config-openapi.yml\n  - openapi/dotdigital-chat-message-openapi.yml\n\
  \  - openapi/dotdigital-chat-openapi.yml\n  - openapi/dotdigital-chat-presence-openapi.yml\n  - openapi/dotdigital-configuration-service-openapi.yml\n  - openapi/dotdigital-contact-data-fields-openapi.yml\n  - openapi/dotdigital-contacts-openapi.yml\n  - openapi/dotdigital-content-openapi.yml\n  - openapi/dotdigital-conversation-message-openapi.yml\n  - openapi/dotdigital-conversation-openapi.yml\n  - openapi/dotdigital-cpaas-openapi.yml\n  - openapi/dotdigital-data-firehose-openapi.yml\n  - openapi/dotdigital-documents-openapi.yml\n  - openapi/dotdigital-ecommerce-openapi.yml\n  - openapi/dotdigital-email-campaigns-openapi.yml\n  - openapi/dotdigital-email-contacts-openapi.yml\n  - openapi/dotdigital-events-openapi.yml\n  - openapi/dotdigital-images-openapi.yml\n  - openapi/dotdigital-insight-and-transactional-data-openapi.yml\n  - openapi/dotdigital-insight-data-service-openapi.yml\n  - openapi/dotdigital-lists-address-books-openapi.yml\n  - openapi/dotdigital-marketing-email-openapi.yml\n\
  \  - openapi/dotdigital-message-history-openapi.yml\n  - openapi/dotdigital-message-rules-openapi.yml\n  - openapi/dotdigital-omnichannel-openapi.yml\n  - openapi/dotdigital-pages-and-forms-openapi.yml\n  - openapi/dotdigital-phone-number-validation-openapi.yml\n  - openapi/dotdigital-preferences-and-subscriptions-openapi.yml\n  - openapi/dotdigital-product-recommendations-openapi.yml\n  - openapi/dotdigital-profile-openapi.yml\n  - openapi/dotdigital-programs-openapi.yml\n  - openapi/dotdigital-scoring-openapi.yml\n  - openapi/dotdigital-segments-openapi.yml\n  - openapi/dotdigital-session-openapi.yml\n  - openapi/dotdigital-sms-campaigns-openapi.yml\n  - openapi/dotdigital-templates-openapi.yml\n  - openapi/dotdigital-transactional-email-openapi.yml\n  - openapi/dotdigital-webhook-openapi.yml\n  - openapi/dotdigital-whatsapp-channel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/authentication/dotdigital-authentication.yml
summary_line: http · 1 scheme
tags:
- Marketing Automation
- Email Marketing
- SMS
- MMS
- WhatsApp
- Contacts
- Campaigns
- Push Notifications
- Transactional Email
- Engagement
- Automation
- CPaaS
- Omnichannel
- Customer Data
- Consent Management
- Personalization
- Loyalty
- E-Commerce
- Event
- Webhook
---
