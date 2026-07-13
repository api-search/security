---
api_specs:
- filename: follow-up-boss-openapi.yml
  format: yaml
  label: Follow Up Boss API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/openapi/follow-up-boss-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: followupboss.com
  spf: true
hosts:
- cert_expires: Sep 28 23:11:55 2026 GMT
  host: www.followupboss.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 08:31:05 2026 GMT
  host: docs.followupboss.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: api.followupboss.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Follow Up Boss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Follow Up Boss, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Follow Up Boss
provider_slug: follow-up-boss
slug: follow-up-boss-domain-security
source_filename: follow-up-boss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.followupboss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:11:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.followupboss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 08:31:05 2026 GMT\n  hsts: null\n- host: api.followupboss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: followupboss.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/follow-up-boss/refs/heads/main/security/follow-up-boss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- CRM
- Lead Management
- Sales Automation
- Follow Up
- Pipeline Management
---
