---
api_specs:
- filename: localytics-campaigns-audiences-openapi.yml
  format: yaml
  label: Localytics Campaigns And Audience API
  slug: localytics-campaigns-and-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-campaigns-audiences-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: localytics.com
  spf: true
hosts:
- cert_expires: Aug 23 09:59:33 2026 GMT
  host: www.localytics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: dashboard.localytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Localytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Localytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Localytics
provider_slug: localytics
slug: localytics-domain-security
source_filename: localytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.localytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:59:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dashboard.localytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: localytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/security/localytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Mobile Analytics
- Push Notifications
- Customer Engagement
- Marketing Automation
- APIs
---
