---
api_specs:
- filename: cisco-webex-admin-openapi.json
  format: json
  label: Cisco Webex Administration API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-admin-openapi.json
- filename: cisco-webex-broadworks-openapi.json
  format: json
  label: Cisco Webex BroadWorks API
  slug: broadworks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-broadworks-openapi.json
- filename: cisco-webex-cloud-calling-openapi.json
  format: json
  label: Cisco Webex Cloud Calling API
  slug: cloud-calling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-cloud-calling-openapi.json
- filename: cisco-webex-contact-center-openapi.json
  format: json
  label: Cisco Webex Contact Center API
  slug: contact-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-contact-center-openapi.json
- filename: cisco-webex-device-openapi.json
  format: json
  label: Cisco Webex Devices API
  slug: device
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-device-openapi.json
- filename: cisco-webex-meeting-openapi.json
  format: json
  label: Cisco Webex Meetings API
  slug: meeting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-meeting-openapi.json
- filename: cisco-webex-messaging-openapi.json
  format: json
  label: Cisco Webex Messaging API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-messaging-openapi.json
- filename: cisco-webex-ucm-openapi.json
  format: json
  label: Cisco Webex Unified CM API
  slug: ucm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-ucm-openapi.json
- filename: cisco-webex-wholesale-openapi.json
  format: json
  label: Cisco Webex Wholesale API
  slug: wholesale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-wholesale-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "identrust.com"
  - 128 issuewild "digicert.com"
  - 128 issuewild "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webex.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: webexapis.com
  spf: false
hosts:
- cert_expires: Dec 21 09:08:54 2026 GMT
  host: developer.webex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 17:46:40 2027 GMT
  host: www.webex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 08:51:15 2026 GMT
  host: webexapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Webex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Webex, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Webex
provider_slug: cisco-webex
slug: cisco-webex-domain-security
source_filename: cisco-webex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 17:46:40 2027 GMT\n  hsts: null\n- host: webexapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:51:15 2026 GMT\n  hsts: null\ndomains:\n- domain: webex.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  - 128 issuewild \"digicert.com\"\n  - 128 issuewild \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: webexapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/security/cisco-webex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
---
