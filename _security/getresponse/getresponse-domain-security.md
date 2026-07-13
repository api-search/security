---
api_specs:
- filename: getresponse-openapi.yml
  format: yaml
  label: GetResponse API v3
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/openapi/getresponse-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "certum.pl"
  - 0 issuewild "certum.pl"
  - 0 issue "godaddy.com"
  - 0 issue "rapidssl.com"
  - 0 issue "digicert.com"
  - 0 issuewild "rapidssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getresponse.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.getresponse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: apireference.getresponse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.getresponse.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getresponse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetResponse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GetResponse
provider_slug: getresponse
slug: getresponse-domain-security
source_filename: getresponse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getresponse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apireference.getresponse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.getresponse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getresponse.com\n  dnssec: false\n  caa:\n  - 0 issue \"certum.pl\"\n  - 0 issuewild \"certum.pl\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"rapidssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getresponse/refs/heads/main/security/getresponse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Marketing Automation
- Landing Pages
- Webinars
- Conversion Funnels
- CRM
---
