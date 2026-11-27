---
api_specs:
- filename: google-chrome-challenge-api-openapi.yml
  format: yaml
  label: Google Chrome Challenge API
  slug: google-chrome-challenge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-challenge-api-openapi.yml
- filename: google-chrome-customers-api-openapi.yml
  format: yaml
  label: Google Chrome Customers API
  slug: google-chrome-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-customers-api-openapi.yml
- filename: google-chrome-media-api-openapi.yml
  format: yaml
  label: Google Chrome Media API
  slug: google-chrome-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-media-api-openapi.yml
- filename: google-chrome-operations-api-openapi.yml
  format: yaml
  label: Google Chrome Operations API
  slug: google-chrome-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-operations-api-openapi.yml
- filename: google-chrome-platforms-api-openapi.yml
  format: yaml
  label: Google Chrome Platforms API
  slug: google-chrome-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-platforms-api-openapi.yml
- filename: google-chrome-publishers-api-openapi.yml
  format: yaml
  label: Google Chrome Publishers API
  slug: google-chrome-publishers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-publishers-api-openapi.yml
- filename: google-chrome-records-api-openapi.yml
  format: yaml
  label: Google Chrome Records API
  slug: google-chrome-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-records-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: chromeenterprise.google
  spf: false
hosts:
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:46 2026 GMT
  host: chromeenterprise.google
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: chromemanagement.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Chrome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Chrome, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Chrome
provider_slug: google-chrome
slug: google-chrome-domain-security
source_filename: google-chrome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: false\n- host: chromeenterprise.google\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:46 2026 GMT\n  hsts: false\n- host: chromemanagement.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: chromeenterprise.google\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/google-chrome/security/google-chrome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Browser
- Chrome Extensions
- Developer Tools
- Web Platform
---
