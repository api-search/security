---
api_specs:
- filename: canada-health-infoway-capabilitystatement-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Capability Statement API
  slug: canada-health-infoway-capabilitystatement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-capabilitystatement-api-openapi.yml
- filename: canada-health-infoway-codesystem-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Code System API
  slug: canada-health-infoway-codesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-codesystem-api-openapi.yml
- filename: canada-health-infoway-codesystems-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Codesystems API
  slug: canada-health-infoway-codesystems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-codesystems-api-openapi.yml
- filename: canada-health-infoway-conceptmap-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Concept Map API
  slug: canada-health-infoway-conceptmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-conceptmap-api-openapi.yml
- filename: canada-health-infoway-maps-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Maps API
  slug: canada-health-infoway-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-maps-api-openapi.yml
- filename: canada-health-infoway-notification-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Notification API
  slug: canada-health-infoway-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-notification-api-openapi.yml
- filename: canada-health-infoway-packages-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Packages API
  slug: canada-health-infoway-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-packages-api-openapi.yml
- filename: canada-health-infoway-resourcelocations-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Resourcelocations API
  slug: canada-health-infoway-resourcelocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-resourcelocations-api-openapi.yml
- filename: canada-health-infoway-session-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Session API
  slug: canada-health-infoway-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-session-api-openapi.yml
- filename: canada-health-infoway-subsets-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Subsets API
  slug: canada-health-infoway-subsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-subsets-api-openapi.yml
- filename: canada-health-infoway-valueset-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Value Set API
  slug: canada-health-infoway-valueset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-valueset-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: infoway-inforoute.ca
  spf: false
hosts:
- cert_expires: Aug 29 19:48:47 2026 GMT
  host: www.infoway-inforoute.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 07:45:56 2026 GMT
  host: termapi.infoway-inforoute.ca
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Canada Health Infoway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canada Health Infoway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Canada Health Infoway
provider_slug: canada-health-infoway
slug: canada-health-infoway-domain-security
source_filename: canada-health-infoway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infoway-inforoute.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 19:48:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: termapi.infoway-inforoute.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 07:45:56 2026 GMT\n  hsts: null\ndomains:\n- domain: infoway-inforoute.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/security/canada-health-infoway-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Healthcare
- Canada
- FHIR
- HL7
- Interoperability
- Terminology
- National Health System
- Digital Health
- Standards
- CA Core
---
