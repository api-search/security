---
api_specs:
- filename: google-chrome-management-api-openapi.json
  format: json
  label: Chrome Management API
  slug: chrome-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-management-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chromeenterprise.google
  spf: false
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:38:10 2026 GMT
  host: chromeenterprise.google
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: chromemanagement.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Chrome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Chrome, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Google Chrome
provider_slug: google-chrome
slug: google-chrome-domain-security
source_filename: google-chrome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chromeenterprise.google\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:38:10 2026 GMT\n  hsts: false\n- host: chromemanagement.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: chromeenterprise.google\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/security/google-chrome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Browser
- Chrome Extensions
- Developer Tools
- Web Platform
---
