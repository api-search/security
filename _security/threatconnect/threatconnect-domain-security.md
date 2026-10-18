---
api_specs:
- filename: threatconnect-apps-api-openapi.yml
  format: yaml
  label: ThreatConnect Apps API
  slug: threatconnect-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-apps-api-openapi.yml
- filename: threatconnect-batch-api-openapi.yml
  format: yaml
  label: ThreatConnect Batch API
  slug: threatconnect-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-batch-api-openapi.yml
- filename: threatconnect-cases-api-openapi.yml
  format: yaml
  label: ThreatConnect Cases API
  slug: threatconnect-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-cases-api-openapi.yml
- filename: threatconnect-custommetrics-api-openapi.yml
  format: yaml
  label: ThreatConnect Custommetrics API
  slug: threatconnect-custommetrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-custommetrics-api-openapi.yml
- filename: threatconnect-groups-api-openapi.yml
  format: yaml
  label: ThreatConnect Groups API
  slug: threatconnect-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-groups-api-openapi.yml
- filename: threatconnect-indicators-api-openapi.yml
  format: yaml
  label: ThreatConnect Indicators API
  slug: threatconnect-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-indicators-api-openapi.yml
- filename: threatconnect-notes-api-openapi.yml
  format: yaml
  label: ThreatConnect Notes API
  slug: threatconnect-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-notes-api-openapi.yml
- filename: threatconnect-notifications-api-openapi.yml
  format: yaml
  label: ThreatConnect Notifications API
  slug: threatconnect-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-notifications-api-openapi.yml
- filename: threatconnect-services-api-openapi.yml
  format: yaml
  label: ThreatConnect Services API
  slug: threatconnect-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-services-api-openapi.yml
- filename: threatconnect-tasks-api-openapi.yml
  format: yaml
  label: ThreatConnect Tasks API
  slug: threatconnect-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-tasks-api-openapi.yml
- filename: threatconnect-tc-taxii-api-openapi.yml
  format: yaml
  label: ThreatConnect Tc Taxii API
  slug: threatconnect-tc-taxii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-tc-taxii-api-openapi.yml
- filename: threatconnect-threatconnect-api-api-openapi.yml
  format: yaml
  label: ThreatConnect ThreatConnect API
  slug: threatconnect-threatconnect-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-threatconnect-api-api-openapi.yml
- filename: threatconnect-token-api-openapi.yml
  format: yaml
  label: ThreatConnect Token API
  slug: threatconnect-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-token-api-openapi.yml
- filename: threatconnect-types-api-openapi.yml
  format: yaml
  label: ThreatConnect Types API
  slug: threatconnect-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-types-api-openapi.yml
- filename: threatconnect-victims-api-openapi.yml
  format: yaml
  label: ThreatConnect Victims API
  slug: threatconnect-victims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-victims-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: threatconnect.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: threatconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Threatconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThreatConnect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThreatConnect
provider_slug: threatconnect
slug: threatconnect-domain-security
source_filename: threatconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: threatconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: threatconnect.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/security/threatconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Threat Intelligence
- Security Operations
- Platform
---
