---
description: ''
domains:
- caa:
  - 128 issuewild "identrust.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
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
name: Cisco Webex Meetings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Webex Meetings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Webex Meetings
provider_slug: cisco-webex-meetings
slug: cisco-webex-meetings-domain-security
source_filename: cisco-webex-meetings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: webexapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:51:15 2026 GMT\n  hsts: null\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: webex.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"identrust.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: webexapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex-meetings/refs/heads/main/security/cisco-webex-meetings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Communications
- Enterprise
- Meetings
- Video Conferencing
---
