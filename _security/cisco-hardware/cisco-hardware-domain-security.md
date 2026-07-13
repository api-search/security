---
api_specs:
- filename: openapiSpec
  format: yaml
  label: Cisco Meraki Dashboard API
  slug: meraki-dashboard-api
  spec_type: OpenAPI
  url: https://api.meraki.com/api/v1/openapiSpec
- filename: openapi.yaml
  format: yaml
  label: Cisco Intersight API
  slug: intersight-api
  spec_type: OpenAPI
  url: https://intersight.com/apidocs/downloads/
description: ''
domains:
- caa:
  - 128 issuewild "digicert.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 128 issuewild "identrust.com"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "globalsign.com"
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
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: intersight.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Hardware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Hardware, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Hardware
provider_slug: cisco-hardware
slug: cisco-hardware-domain-security
source_filename: cisco-hardware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.meraki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: intersight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"digicert.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 128 issuewild \"identrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: meraki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/security/cisco-hardware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hardware
- Infrastructure
- Networking
- Routers
- Switches
---
