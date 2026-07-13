---
api_specs:
- filename: cisco-meraki-api.yaml
  format: yaml
  label: Cisco Meraki Dashboard API
  slug: meraki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/openapi/cisco-meraki-api.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 128 issuewild "ssl.com"
  - 0 issue "digicert.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meraki.com
  spf: true
hosts:
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:59:42 2026 GMT
  host: api.meraki.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 09:08:54 2026 GMT
  host: developer.webex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco
provider_slug: cisco
slug: cisco-domain-security
source_filename: cisco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.meraki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: meraki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/security/cisco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- Collaboration
- Enterprise
- Networking
- Security
- SD-WAN
---
