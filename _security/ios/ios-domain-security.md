---
api_specs:
- filename: app-store-connect-openapi.json
  format: json
  label: App Store Connect API
  slug: app-store-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ios/main/openapi/app-store-connect-openapi.json
- filename: app-store-server-notifications-asyncapi.yml
  format: yaml
  label: App Store Server Notifications
  slug: app-store-server-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ios/main/asyncapi/app-store-server-notifications-asyncapi.yml
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
- cert_expires: Jan 20 20:03:56 2027 GMT
  host: api.appstoreconnect.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 18:27:24 2026 GMT
  host: api.storekit.itunes.apple.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iOS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iOS
provider_slug: ios
slug: ios-domain-security
source_filename: ios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.appstoreconnect.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 20:03:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.storekit.itunes.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:27:24 2026 GMT\n  hsts: null\ndomains:\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ios/refs/heads/main/security/ios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- iOS
- Apple
- Mobile
- App Store
- Push Notifications
- In-App Purchases
- Subscriptions
- Authentication
- Wallet
- Developer Platform
---
