---
api_specs:
- filename: act-on-rest-api-openapi.yml
  format: yaml
  label: Act-On REST API
  slug: act-on-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/openapi/act-on-rest-api-openapi.yml
- filename: act-on-custom-objects-service-openapi.yml
  format: yaml
  label: Act-On Custom Objects Service
  slug: act-on-custom-objects-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/openapi/act-on-custom-objects-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: act-on.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: actonsoftware.com
  spf: true
hosts:
- cert_expires: Nov 11 07:00:43 2026 GMT
  host: act-on.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 05:21:36 2026 GMT
  host: developer.act-on.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: restapi.actonsoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Act On Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Act-On, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Act-On
provider_slug: act-on
slug: act-on-domain-security
source_filename: act-on-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: act-on.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 07:00:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.act-on.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:21:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: restapi.actonsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: act-on.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: actonsoftware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/security/act-on-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketing
- Marketing Automation
- Email Marketing
- Email
- Marketing Technology
- Lead Generation
- Campaign Management
- Customer Data
- Webhook
---
