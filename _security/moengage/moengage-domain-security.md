---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moengage.com
  spf: true
hosts:
- cert_expires: Sep 15 10:06:38 2026 GMT
  host: www.moengage.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api-01.moengage.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: pushapi-01.moengage.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Moengage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoEngage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MoEngage
provider_slug: moengage
slug: moengage-domain-security
source_filename: moengage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moengage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:06:38 2026 GMT\n  hsts: false\n- host: api-01.moengage.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\n- host: pushapi-01.moengage.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: moengage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/security/moengage-domain-security.yml
summary_line: TLSv1.3 · DMARC
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
