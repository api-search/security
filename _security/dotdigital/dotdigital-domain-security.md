---
api_specs:
- filename: swagger.json
  format: json
  label: Dotdigital v2 API
  slug: dotdigital-v2-api
  spec_type: OpenAPI
  url: https://r1-api.dotdigital.com/swagger.json
- filename: swagger.json
  format: json
  label: Dotdigital v3 API
  slug: dotdigital-v3-api
  spec_type: OpenAPI
  url: https://r1-api.dotdigital.com/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dotdigital.com
  spf: true
hosts:
- cert_expires: Aug 29 09:19:44 2026 GMT
  host: dotdigital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 09:19:44 2026 GMT
  host: developer.dotdigital.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 09:19:44 2026 GMT
  host: r1-api.dotdigital.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dotdigital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dotdigital, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dotdigital
provider_slug: dotdigital
slug: dotdigital-domain-security
source_filename: dotdigital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dotdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 09:19:44 2026 GMT\n  hsts: false\n- host: developer.dotdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 09:19:44 2026 GMT\n  hsts: null\n- host: r1-api.dotdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 09:19:44 2026 GMT\n  hsts: null\ndomains:\n- domain: dotdigital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/security/dotdigital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing Automation
- Email Marketing
- SMS
- WhatsApp
- Contacts
- Campaigns
- Push Notifications
- Transactional Email
- Engagement
- Automation
---
