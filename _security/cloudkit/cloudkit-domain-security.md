---
api_specs:
- filename: cloudkit-assets-api-openapi.yml
  format: yaml
  label: Apple CloudKit Assets API
  slug: cloudkit-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-assets-api-openapi.yml
- filename: cloudkit-changes-api-openapi.yml
  format: yaml
  label: Apple CloudKit Changes API
  slug: cloudkit-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-changes-api-openapi.yml
- filename: cloudkit-records-api-openapi.yml
  format: yaml
  label: Apple CloudKit Records API
  slug: cloudkit-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-records-api-openapi.yml
- filename: cloudkit-subscriptions-api-openapi.yml
  format: yaml
  label: Apple CloudKit Subscriptions API
  slug: cloudkit-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-subscriptions-api-openapi.yml
- filename: cloudkit-tokens-api-openapi.yml
  format: yaml
  label: Apple CloudKit Tokens API
  slug: cloudkit-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-tokens-api-openapi.yml
- filename: cloudkit-users-api-openapi.yml
  format: yaml
  label: Apple CloudKit Users API
  slug: cloudkit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-users-api-openapi.yml
- filename: cloudkit-zones-api-openapi.yml
  format: yaml
  label: Apple CloudKit Zones API
  slug: cloudkit-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-zones-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: icloud.com
  spf: true
- caa:
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- cert_expires: Jan  7 18:07:22 2027 GMT
  host: www.icloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:10:52 2026 GMT
  host: developer.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 20:54:06 2027 GMT
  host: api.apple-cloudkit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apple CloudKit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apple CloudKit
provider_slug: cloudkit
slug: cloudkit-domain-security
source_filename: cloudkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 18:07:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apple-cloudkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 20:54:06 2027 GMT\n  hsts: null\ndomains:\n- domain: icloud.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/security/cloudkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apple
- Cloud Storage
- CloudKit
- Database
- iCloud
- Mobile
- Sync
- Web Services
---
