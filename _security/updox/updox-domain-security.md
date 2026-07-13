---
api_specs:
- filename: updox-openapi.yml
  format: yaml
  label: Updox Address Book API
  slug: updox-address-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/openapi/updox-openapi.yml
- filename: updox-openapi.yml
  format: yaml
  label: Updox Faxing API
  slug: updox-faxing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/openapi/updox-openapi.yml
- filename: updox-openapi.yml
  format: yaml
  label: Updox Video Chat API
  slug: updox-video-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/openapi/updox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: updox.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: updoxqa.com
  spf: false
hosts:
- cert_expires: Sep 15 05:15:57 2026 GMT
  host: www.updox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 15:40:46 2026 GMT
  host: help.updox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: updoxqa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Updox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Updox, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Updox
provider_slug: updox
slug: updox-domain-security
source_filename: updox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.updox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:15:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.updox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:40:46 2026 GMT\n  hsts: false\n- host: updoxqa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: updox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: updoxqa.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/security/updox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Patient Engagement
- Secure Messaging
- Electronic Fax
- Telehealth
- Document Management
- HIPAA
- EverCommerce
---
