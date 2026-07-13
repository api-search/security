---
api_specs:
- filename: cisco-voice-portal-call-control-openapi.yml
  format: yaml
  label: Cisco Voice Portal Call Control API
  slug: cisco-voice-portal-call-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-call-control-openapi.yml
- filename: cisco-voice-portal-reporting-openapi.yml
  format: yaml
  label: Cisco Voice Portal Reporting API
  slug: cisco-voice-portal-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-reporting-openapi.yml
- filename: cisco-voice-portal-administration-openapi.yml
  format: yaml
  label: Cisco Voice Portal Administration API
  slug: cisco-voice-portal-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-administration-openapi.yml
- filename: cisco-voice-portal-vxml-services-openapi.yml
  format: yaml
  label: Cisco Voice Portal VXML Services API
  slug: cisco-voice-portal-vxml-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-vxml-services-openapi.yml
- filename: cisco-voice-portal-call-events-asyncapi.yml
  format: yaml
  label: Cisco Voice Portal Call Events API
  slug: cisco-voice-portal-call-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/asyncapi/cisco-voice-portal-call-events-asyncapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "identrust.com"
  - 0 issue "digicert.com"
  - 128 issuewild "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
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
name: Cisco Voice Portal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Voice Portal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
slug: cisco-voice-portal-domain-security
source_filename: cisco-voice-portal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"identrust.com\"\n  - 0 issue \"digicert.com\"\n  - 128 issuewild \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/security/cisco-voice-portal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
---
