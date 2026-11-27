---
api_specs:
- filename: mailinapp-com-contacts-api-openapi.yml
  format: yaml
  label: MailInApp Contacts API
  slug: mailinapp-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-contacts-api-openapi.yml
- filename: mailinapp-com-courses-api-openapi.yml
  format: yaml
  label: MailInApp Courses API
  slug: mailinapp-com-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-courses-api-openapi.yml
- filename: mailinapp-com-deals-api-openapi.yml
  format: yaml
  label: MailInApp Deals API
  slug: mailinapp-com-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-deals-api-openapi.yml
- filename: mailinapp-com-experiments-api-openapi.yml
  format: yaml
  label: MailInApp Experiments API
  slug: mailinapp-com-experiments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-experiments-api-openapi.yml
- filename: mailinapp-com-journeys-api-openapi.yml
  format: yaml
  label: MailInApp Journeys API
  slug: mailinapp-com-journeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-journeys-api-openapi.yml
- filename: mailinapp-com-live-view-api-openapi.yml
  format: yaml
  label: MailInApp Live view API
  slug: mailinapp-com-live-view-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-live-view-api-openapi.yml
- filename: mailinapp-com-send-api-openapi.yml
  format: yaml
  label: MailInApp Send API
  slug: mailinapp-com-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-send-api-openapi.yml
- filename: mailinapp-com-webhooks-api-openapi.yml
  format: yaml
  label: MailInApp Webhooks API
  slug: mailinapp-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-webhooks-api-openapi.yml
- filename: mailinapp-com-webinars-api-openapi.yml
  format: yaml
  label: MailInApp Webinars API
  slug: mailinapp-com-webinars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-webinars-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mailinapp.com
  spf: true
hosts:
- cert_expires: Jan 28 14:34:28 2027 GMT
  host: mailinapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MailInApp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailInApp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MailInApp
provider_slug: mailinapp-com
slug: mailinapp-com-domain-security
source_filename: mailinapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailinapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 14:34:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailinapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mailinapp-com/security/mailinapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Marketing
- Interactive
- Software-as-a-Service
---
