---
api_specs:
- filename: freshsales-openapi.yml
  format: yaml
  label: Freshsales CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freshworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myfreshworks.com
  spf: true
hosts:
- cert_expires: Aug 22 10:30:03 2026 GMT
  host: www.freshworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: developers.freshworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <bundle-alias>.myfreshworks.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<bundle-ali'
kind: domain-security
layout: security
method: probed
name: Freshsales Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freshsales, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freshsales
provider_slug: freshsales
slug: freshsales-domain-security
source_filename: freshsales-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freshworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:30:03 2026 GMT\n  hsts: null\n- host: developers.freshworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <bundle-alias>.myfreshworks.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<bundle-ali'\n  hsts: null\ndomains:\n- domain: freshworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: myfreshworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/security/freshsales-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- Contacts
- Deals
- Pipeline
- Lead Management
- Freshworks
---
