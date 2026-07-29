---
api_specs:
- filename: marriott-tip-internet-portal-api-openapi.json
  format: json
  label: Marriott TIP Internet Portal API
  slug: marriott-tip-internet-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-tip-internet-portal-api-openapi.json
- filename: marriott-loyalty-account-merge-api-openapi.json
  format: json
  label: Marriott Loyalty Account Merge API
  slug: marriott-loyalty-account-merge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-loyalty-account-merge-api-openapi.json
- filename: marriott-data-collection-api-openapi.json
  format: json
  label: Marriott Data Collection API
  slug: marriott-data-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-collection-api-openapi.json
- filename: marriott-commerce-payment-processor-api-openapi.json
  format: json
  label: Marriott Commerce Payment Processor API
  slug: marriott-commerce-payment-processor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-commerce-payment-processor-api-openapi.json
- filename: marriott-finance-status-notifier-api-openapi.json
  format: json
  label: Marriott Finance Status Notifier API
  slug: marriott-finance-status-notifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-finance-status-notifier-api-openapi.json
- filename: marriott-hotel-operations-ara-api-openapi.json
  format: json
  label: Marriott Hotel Operations ARA Preview Submit API
  slug: marriott-hotel-operations-ara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-hotel-operations-ara-api-openapi.json
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
