---
api_specs:
- filename: webex-messaging-openapi.json
  format: json
  label: Webex Messaging
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-messaging-openapi.json
- filename: webex-meeting-openapi.json
  format: json
  label: Webex Meetings
  slug: meetings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-meeting-openapi.json
- filename: webex-admin-openapi.json
  format: json
  label: Webex Admin
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-admin-openapi.json
- filename: webex-cloud-calling-openapi.json
  format: json
  label: Webex Cloud Calling
  slug: cloud-calling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-cloud-calling-openapi.json
- filename: webex-contact-center-openapi.json
  format: json
  label: Webex Contact Center
  slug: contact-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-contact-center-openapi.json
- filename: webex-device-openapi.json
  format: json
  label: Webex Devices
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-device-openapi.json
- filename: webex-broadworks-openapi.json
  format: json
  label: Webex Broadworks Calling
  slug: broadworks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-broadworks-openapi.json
- filename: webex-ucm-openapi.json
  format: json
  label: Webex for UCM
  slug: ucm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-ucm-openapi.json
- filename: webex-wholesale-openapi.json
  format: json
  label: Webex Wholesale
  slug: wholesale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-wholesale-openapi.json
description: ''
domains:
- caa:
  - 128 issuewild "digicert.com"
  - 128 issuewild "identrust.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webex.com
  spf: true
hosts:
- cert_expires: Oct 10 13:34:52 2026 GMT
  host: developer.webex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Webex
provider_slug: webex
slug: webex-domain-security
source_filename: webex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 13:34:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: webex.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"digicert.com\"\n  - 128 issuewild \"identrust.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/security/webex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calling
- Collaboration
- Communication
- Enterprise
- Messaging
- Video Conferencing
---
