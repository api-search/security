---
api_specs:
- filename: vibes-platform-openapi.yml
  format: yaml
  label: Vibes Platform API
  slug: vibes-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-openapi.yml
- filename: vibes-connect-openapi.yml
  format: yaml
  label: Vibes Connect API
  slug: vibes-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-connect-openapi.yml
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
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer-platform.vibes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:52:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer-aggregation.vibes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer-rbm.vibes.com\n  https: false\ndomains:\n- domain: vibes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
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
