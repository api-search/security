---
api_specs:
- filename: openapi.json
  format: json
  label: Cisco Directory Connector Sync API
  slug: cisco-directory-connector-sync-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Control Hub API
  slug: webex-control-hub-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
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
hosts:
- cert_expires: Dec 21 09:08:54 2026 GMT
  host: developer.webex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 01:46:22 2026 GMT
  host: www.cisco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 09:59:33 2026 GMT
  host: admin.webex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Directory Connector Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Directory Connector, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Directory Connector
provider_slug: cisco-directory-connector
slug: cisco-directory-connector-domain-security
source_filename: cisco-directory-connector-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: admin.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 09:59:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: webex.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"identrust.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"digicert.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  -\
  \ 128 issuewild \"identrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-directory-connector/refs/heads/main/security/cisco-directory-connector-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Active Directory
- Directory
- Enterprise
- Identity Management
- LDAP
- Provisioning
- SCIM
- Synchronization
---
