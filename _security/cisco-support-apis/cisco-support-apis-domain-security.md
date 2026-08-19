---
description: ''
domains:
- caa:
  - 128 issuewild "identrust.com"
  - 0 issue "globalsign.com"
  - 128 issuewild "ssl.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
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
- cert_expires: Nov 24 16:35:02 2026 GMT
  host: apix.cisco.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cisco Support Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Support APIs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Support APIs
provider_slug: cisco-support-apis
slug: cisco-support-apis-domain-security
source_filename: cisco-support-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: apix.cisco.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 16:35:02 2026 GMT\n  hsts: null\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"identrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-support-apis/refs/heads/main/security/cisco-support-apis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Support
- Lifecycle
- Asset Management
- Entitlement
- Enterprise
- Networking
- End of Life
- Defects
- Case Management
- Software Distribution
- RMA
- Smart Net Total Care
---
