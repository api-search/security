---
api_specs:
- filename: openapi.json
  format: json
  label: Webex APIs
  slug: webex-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "identrust.com"
  - 128 issuewild "digicert.com"
  - 128 issuewild "identrust.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 0 issue "globalsign.com"
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
- cert_expires: Dec 21 08:51:15 2026 GMT
  host: webexapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Collaboration Hybrid Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Collaboration Hybrid Solutions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Collaboration Hybrid Solutions
provider_slug: cisco-collaboration-hybrid-solutions
slug: cisco-collaboration-hybrid-solutions-domain-security
source_filename: cisco-collaboration-hybrid-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: webexapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:51:15 2026 GMT\n  hsts: null\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: webex.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  - 128 issuewild \"digicert.com\"\n  - 128 issuewild \"identrust.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: webexapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/security/cisco-collaboration-hybrid-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calling
- Collaboration
- Hybrid Cloud
- Meetings
- Messaging
- Unified Communications
- Webex
---
