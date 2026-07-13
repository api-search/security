---
api_specs:
- filename: appcues-openapi.yml
  format: yaml
  label: Appcues Public API
  slug: appcues-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appcues.com
  spf: true
hosts:
- cert_expires: Oct  3 01:45:28 2026 GMT
  host: www.appcues.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.appcues.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.eu.appcues.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Appcues Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appcues, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Appcues
provider_slug: appcues
slug: appcues-domain-security
source_filename: appcues-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appcues.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:45:28 2026 GMT\n  hsts: false\n- host: api.appcues.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.eu.appcues.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: appcues.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/security/appcues-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Product
- Onboarding
- In-App Guidance
- Analytics
- Customer Success
---
