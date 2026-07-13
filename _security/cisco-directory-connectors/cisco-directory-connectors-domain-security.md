---
api_specs:
- filename: cisco-directory-connectors-openapi.yml
  format: yaml
  label: Cisco Directory Connector API
  slug: cisco-directory-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-directory-connectors/refs/heads/main/openapi/cisco-directory-connectors-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "identrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 128 issuewild "digicert.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: webexapis.com
  spf: false
hosts:
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
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
name: Cisco Directory Connectors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Directory Connectors, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Directory Connectors
provider_slug: cisco-directory-connectors
slug: cisco-directory-connectors-domain-security
source_filename: cisco-directory-connectors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: webexapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:51:15 2026 GMT\n  hsts: null\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"identrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 128 issuewild \"digicert.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: webexapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-directory-connectors/refs/heads/main/security/cisco-directory-connectors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Active Directory
- Directory Services
- Identity Management
- LDAP
- User Synchronization
---
