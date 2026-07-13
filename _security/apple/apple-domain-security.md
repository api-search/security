---
api_specs:
- filename: app-store-connect-openapi-specification.zip
  format: yaml
  label: App Store Connect API
  slug: app-store-connect-api
  spec_type: OpenAPI
  url: https://developer.apple.com/sample-code/app-store-connect/app-store-connect-openapi-specification.zip
description: ''
domains:
- caa:
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  - 0 iodef "mailto:contact_pki@apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- cert_expires: Aug 27 17:10:52 2026 GMT
  host: developer.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 19:46:05 2027 GMT
  host: api.music.apple.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 20:57:12 2026 GMT
  host: weatherkit.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apple, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apple
provider_slug: apple
slug: apple-domain-security
source_filename: apple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.music.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 19:46:05 2027 GMT\n  hsts: null\n- host: weatherkit.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 20:57:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/security/apple-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
- Fortune 100
---
