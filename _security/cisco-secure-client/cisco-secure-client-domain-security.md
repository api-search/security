---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "identrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 128 issuewild "identrust.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: umbrella.com
  spf: true
hosts:
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 20:07:28 2026 GMT
  host: api.umbrella.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: duo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Secure Client Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Secure Client, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Secure Client
provider_slug: cisco-secure-client
slug: cisco-secure-client-domain-security
source_filename: cisco-secure-client-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.umbrella.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:07:28 2026 GMT\n  hsts: null\n- host: duo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 128 issuewild \"identrust.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: umbrella.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0\
  \ issue \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/security/cisco-secure-client-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Endpoint Security
- Remote Access
- Security
- VPN
- Zero Trust
---
