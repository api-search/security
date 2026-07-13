---
api_specs:
- filename: cisco-systems-cisco-api-openapi.yml
  format: yaml
  label: Cisco DevNet API Catalog
  slug: devnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-systems/refs/heads/main/openapi/cisco-systems-cisco-api-openapi.yml
- filename: openapiSpec
  format: yaml
  label: Cisco Meraki Dashboard
  slug: meraki
  spec_type: OpenAPI
  url: https://api.meraki.com/api/v1/openapiSpec
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "identrust.com"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 128 iodef "mailto:infosec@cisco.com"
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
- cert_expires: Nov  9 01:46:22 2026 GMT
  host: www.cisco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Cisco Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Systems
provider_slug: cisco-systems
slug: cisco-systems-domain-security
source_filename: cisco-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:46:22 2026 GMT\n  hsts: null\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.meraki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: meraki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-systems/refs/heads/main/security/cisco-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Infrastructure
- Networking
- Security
- Fortune 100
---
