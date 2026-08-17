---
api_specs:
- filename: vibes-platform-api-openapi.json
  format: json
  label: Vibes Platform API
  slug: vibes-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-api-openapi.json
- filename: vibes-platform-rcs-business-messaging-openapi.json
  format: json
  label: Vibes RCS Business Messaging API
  slug: vibes-rcs-business-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-rcs-business-messaging-openapi.json
- filename: vibes-platform-acquisition-campaigns-api-openapi.yml
  format: yaml
  label: Vibes Platform Acquisition Campaigns API
  slug: vibes-platform-acquisition-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-acquisition-campaigns-api-openapi.yml
- filename: vibes-platform-broadcasts-api-openapi.yml
  format: yaml
  label: Vibes Platform Broadcasts API
  slug: vibes-platform-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-broadcasts-api-openapi.yml
- filename: vibes-platform-callbacks-api-openapi.yml
  format: yaml
  label: Vibes Platform Callbacks API
  slug: vibes-platform-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-callbacks-api-openapi.yml
- filename: vibes-platform-carrier-lookup-api-openapi.yml
  format: yaml
  label: Vibes Platform Carrier Lookup API
  slug: vibes-platform-carrier-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-carrier-lookup-api-openapi.yml
- filename: vibes-platform-events-api-openapi.yml
  format: yaml
  label: Vibes Platform Events API
  slug: vibes-platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-events-api-openapi.yml
- filename: vibes-platform-inbound-messages-api-openapi.yml
  format: yaml
  label: Vibes Platform Inbound Messages API
  slug: vibes-platform-inbound-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-inbound-messages-api-openapi.yml
- filename: vibes-platform-messages-api-openapi.yml
  format: yaml
  label: Vibes Platform Messages API
  slug: vibes-platform-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-messages-api-openapi.yml
- filename: vibes-platform-persons-api-openapi.yml
  format: yaml
  label: Vibes Platform Persons API
  slug: vibes-platform-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-persons-api-openapi.yml
- filename: vibes-platform-subscription-lists-api-openapi.yml
  format: yaml
  label: Vibes Platform Subscription Lists API
  slug: vibes-platform-subscription-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-subscription-lists-api-openapi.yml
- filename: vibes-platform-wallet-passes-api-openapi.yml
  format: yaml
  label: Vibes Platform Wallet Passes API
  slug: vibes-platform-wallet-passes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-wallet-passes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vibes.com
  spf: true
hosts:
- cert_expires: Oct  3 16:52:42 2026 GMT
  host: developer-platform.vibes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:14:44 2026 GMT
  host: developer-aggregation.vibes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer-rbm.vibes.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vibes Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vibes Platform, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vibes Platform
provider_slug: vibes-platform
slug: vibes-platform-domain-security
source_filename: vibes-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer-platform.vibes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:52:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer-aggregation.vibes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer-rbm.vibes.com\n  https: false\ndomains:\n- domain: vibes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/security/vibes-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile Marketing
- Mobile Messaging
- Push Notifications
- SMS
- MMS
- Broadcast Messaging
- Acquisition Campaigns
- Subscription Management
- Wallet Passes
- RCS
---
