---
api_specs:
- filename: marriott-actuator-api-openapi.yml
  format: yaml
  label: Marriott International Actuator API
  slug: marriott-actuator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-actuator-api-openapi.yml
- filename: marriott-auth-api-openapi.yml
  format: yaml
  label: Marriott International Auth API
  slug: marriott-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-auth-api-openapi.yml
- filename: marriott-data-api-openapi.yml
  format: yaml
  label: Marriott International Data API
  slug: marriott-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-api-openapi.yml
- filename: marriott-data-collection-event-api-openapi.yml
  format: yaml
  label: Marriott International Data Collection Event API
  slug: marriott-data-collection-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-collection-event-api-openapi.yml
- filename: marriott-freedompay-freeway-service-api-openapi.yml
  format: yaml
  label: Marriott International FreedomPay Freeway Service API
  slug: marriott-freedompay-freeway-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-freedompay-freeway-service-api-openapi.yml
- filename: marriott-guest-validation-api-openapi.yml
  format: yaml
  label: Marriott International Guest Validation API
  slug: marriott-guest-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-guest-validation-api-openapi.yml
- filename: marriott-internet-purchase-update-api-openapi.yml
  format: yaml
  label: Marriott International Internet Purchase Update API
  slug: marriott-internet-purchase-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-internet-purchase-update-api-openapi.yml
- filename: marriott-landing-page-api-openapi.yml
  format: yaml
  label: Marriott International Landing Page API
  slug: marriott-landing-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-landing-page-api-openapi.yml
- filename: marriott-loyalty-api-openapi.yml
  format: yaml
  label: Marriott International Loyalty API
  slug: marriott-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-loyalty-api-openapi.yml
- filename: marriott-postpreviewsubmit-api-openapi.yml
  format: yaml
  label: Marriott International Post Preview Submit API
  slug: marriott-postpreviewsubmit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-postpreviewsubmit-api-openapi.yml
- filename: marriott-retrieveconfigsmonitoredbyconfigwatcher-api-openapi.yml
  format: yaml
  label: Marriott International Retrieve Configs Monitored By Config Watcher API
  slug: marriott-retrieveconfigsmonitoredbyconfigwatcher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-retrieveconfigsmonitoredbyconfigwatcher-api-openapi.yml
- filename: marriott-status-api-openapi.yml
  format: yaml
  label: Marriott International Status API
  slug: marriott-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marriott.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.marriott.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: virtserver.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marriott Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marriott International, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Marriott International
provider_slug: marriott
slug: marriott-domain-security
source_filename: marriott-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marriott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\n- host: api.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: virtserver.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: marriott.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/security/marriott-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Distribution
- Loyalty
- Short Term Rental
- Corporate Travel
---
