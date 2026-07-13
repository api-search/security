---
api_specs:
- filename: snaplogic-public-apis-openapi.yml
  format: yaml
  label: SnapLogic Public APIs
  slug: snaplogic-public-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaplogic/refs/heads/main/openapi/snaplogic-public-apis-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snaplogic.com
  spf: true
hosts:
- cert_expires: Sep 25 09:32:16 2026 GMT
  host: www.snaplogic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 00:57:08 2026 GMT
  host: docs.snaplogic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 07:24:47 2026 GMT
  host: developer.snaplogic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snaplogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SnapLogic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SnapLogic
provider_slug: snaplogic
slug: snaplogic-domain-security
source_filename: snaplogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.snaplogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:32:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.snaplogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 00:57:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.snaplogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:24:47 2026 GMT\n  hsts: false\ndomains:\n- domain: snaplogic.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snaplogic/refs/heads/main/security/snaplogic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- API Management
- Automation
- Data Integration
- Integrations
- iPaaS
- Management
---
