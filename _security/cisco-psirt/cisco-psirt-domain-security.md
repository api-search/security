---
api_specs:
- filename: cisco-psirt-current-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Current Endpoints API
  slug: cisco-psirt-current-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-current-endpoints-api-openapi.yml
- filename: cisco-psirt-obsolete-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Obsolete Endpoints API
  slug: cisco-psirt-obsolete-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml
- filename: cisco-psirt-sunset-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Sunset Endpoints API
  slug: cisco-psirt-sunset-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-sunset-endpoints-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "ssl.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 128 issuewild "identrust.com"
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
kind: domain-security
layout: security
method: probed
name: Cisco Psirt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco PSIRT openVuln API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco PSIRT openVuln API
provider_slug: cisco-psirt
slug: cisco-psirt-domain-security
source_filename: cisco-psirt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 128 issuewild \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/security/cisco-psirt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Vulnerability Management
- Threat Intelligence
- Disclosure
- Compliance
- Networking
---
