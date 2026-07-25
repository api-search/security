---
api_specs:
- filename: cisco-expressway-admin-account-api-openapi.yml
  format: yaml
  label: Cisco Expressway Admin Account API
  slug: cisco-expressway-admin-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-admin-account-api-openapi.yml
- filename: cisco-expressway-alarms-api-openapi.yml
  format: yaml
  label: Cisco Expressway Alarms API
  slug: cisco-expressway-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-alarms-api-openapi.yml
- filename: cisco-expressway-calls-api-openapi.yml
  format: yaml
  label: Cisco Expressway Calls API
  slug: cisco-expressway-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-calls-api-openapi.yml
- filename: cisco-expressway-dns-api-openapi.yml
  format: yaml
  label: Cisco Expressway DNS API
  slug: cisco-expressway-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-dns-api-openapi.yml
- filename: cisco-expressway-licensing-api-openapi.yml
  format: yaml
  label: Cisco Expressway Licensing API
  slug: cisco-expressway-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-licensing-api-openapi.yml
- filename: cisco-expressway-ntp-api-openapi.yml
  format: yaml
  label: Cisco Expressway NTP API
  slug: cisco-expressway-ntp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-ntp-api-openapi.yml
- filename: cisco-expressway-registrations-api-openapi.yml
  format: yaml
  label: Cisco Expressway Registrations API
  slug: cisco-expressway-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-registrations-api-openapi.yml
- filename: cisco-expressway-resource-usage-api-openapi.yml
  format: yaml
  label: Cisco Expressway Resource Usage API
  slug: cisco-expressway-resource-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-resource-usage-api-openapi.yml
- filename: cisco-expressway-search-rules-api-openapi.yml
  format: yaml
  label: Cisco Expressway Search Rules API
  slug: cisco-expressway-search-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-search-rules-api-openapi.yml
- filename: cisco-expressway-sftp-api-openapi.yml
  format: yaml
  label: Cisco Expressway SFTP API
  slug: cisco-expressway-sftp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-sftp-api-openapi.yml
- filename: cisco-expressway-sip-api-openapi.yml
  format: yaml
  label: Cisco Expressway SIP API
  slug: cisco-expressway-sip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-sip-api-openapi.yml
- filename: cisco-expressway-system-api-openapi.yml
  format: yaml
  label: Cisco Expressway System API
  slug: cisco-expressway-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-system-api-openapi.yml
- filename: cisco-expressway-system-status-api-openapi.yml
  format: yaml
  label: Cisco Expressway System Status API
  slug: cisco-expressway-system-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-system-status-api-openapi.yml
- filename: cisco-expressway-transforms-api-openapi.yml
  format: yaml
  label: Cisco Expressway Transforms API
  slug: cisco-expressway-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-transforms-api-openapi.yml
- filename: cisco-expressway-upgrade-api-openapi.yml
  format: yaml
  label: Cisco Expressway Upgrade API
  slug: cisco-expressway-upgrade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-upgrade-api-openapi.yml
- filename: cisco-expressway-zones-api-openapi.yml
  format: yaml
  label: Cisco Expressway Zones API
  slug: cisco-expressway-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-zones-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "ssl.com"
  - 0 issue "digicert.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
hosts:
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 01:46:22 2026 GMT
  host: www.cisco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Expressway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Expressway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Expressway
provider_slug: cisco-expressway
slug: cisco-expressway-domain-security
source_filename: cisco-expressway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/security/cisco-expressway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
---
