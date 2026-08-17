---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dotdigital.com
  spf: true
hosts:
- cert_expires: Feb 25 10:52:02 2027 GMT
  host: dotdigital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 10:52:02 2027 GMT
  host: developer.dotdigital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 10:52:02 2027 GMT
  host: r1-api.dotdigital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dotdigital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dotdigital, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dotdigital
provider_slug: dotdigital
slug: dotdigital-domain-security
source_filename: dotdigital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dotdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 10:52:02 2027 GMT\n  hsts: false\n- host: developer.dotdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 10:52:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: r1-api.dotdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 10:52:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dotdigital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/security/dotdigital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
- Ecommerce
- Events
- Webhooks
---
