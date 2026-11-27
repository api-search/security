---
api_specs:
- filename: free-sign-com-consent-api-openapi.yml
  format: yaml
  label: FreeSign Consent API
  slug: free-sign-com-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/free-sign-com/openapi/free-sign-com-consent-api-openapi.yml
- filename: free-sign-com-envelopes-api-openapi.yml
  format: yaml
  label: FreeSign Envelopes API
  slug: free-sign-com-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/free-sign-com/openapi/free-sign-com-envelopes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: free-sign.com
  spf: true
hosts:
- cert_expires: Dec 12 00:16:46 2026 GMT
  host: free-sign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FreeSign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeSign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FreeSign
provider_slug: free-sign-com
slug: free-sign-com-domain-security
source_filename: free-sign-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: free-sign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 00:16:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: free-sign.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/free-sign-com/security/free-sign-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- FreeSoftware
- BrowserApp
- Open Source
---
