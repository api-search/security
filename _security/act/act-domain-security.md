---
api_specs:
- filename: index.html
  format: yaml
  label: Act! Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://apimta.act.com/act.web.api/swagger/index.html
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "networksolutions.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: act.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.act.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: developer.act.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: apimta.act.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Act Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Act! CRM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Act! CRM
provider_slug: act
slug: act-domain-security
source_filename: act-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.act.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\n- host: developer.act.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\n- host: apimta.act.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: act.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"networksolutions.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/security/act-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Customer Relationship Management
- Marketing Automation
- Contact Management
- Sales
- Swiftpage
---
