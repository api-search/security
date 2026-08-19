---
api_specs:
- filename: cisco-catalyst-center-aaaservices-openapi.yml
  format: yaml
  label: Cisco Catalyst Center Assurance & Intent API
  slug: cisco-catalyst-center-assurance-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-center/refs/heads/main/openapi/cisco-catalyst-center-aaaservices-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 128 issuewild "digicert.com"
  - 128 issuewild "identrust.com"
  - 128 issuewild "ssl.com"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
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
name: Cisco Catalyst Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Catalyst Center, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Catalyst Center
provider_slug: cisco-catalyst-center
slug: cisco-catalyst-center-domain-security
source_filename: cisco-catalyst-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 128 issuewild \"digicert.com\"\n  - 128 issuewild \"identrust.com\"\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-center/refs/heads/main/security/cisco-catalyst-center-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Network Automation
- Intent-Based Networking
- Networking
- Assurance
- Enterprise
- Campus
- Wireless
- SD-Access
- Network Management
- Observability
- Telemetry
- MCP
- Agent Native
- Cisco
---
