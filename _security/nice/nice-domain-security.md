---
api_specs:
- filename: nice-channels-api-openapi.yml
  format: yaml
  label: NICE Channels API
  slug: nice-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-channels-api-openapi.yml
- filename: nice-contacts-api-openapi.yml
  format: yaml
  label: NICE Contacts API
  slug: nice-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-contacts-api-openapi.yml
- filename: nice-incontactapi-api-openapi.yml
  format: yaml
  label: NICE Incontactapi API
  slug: nice-incontactapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-incontactapi-api-openapi.yml
- filename: nice-perform-action-api-openapi.yml
  format: yaml
  label: NICE Perform Action API
  slug: nice-perform-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-perform-action-api-openapi.yml
- filename: nice-result-api-openapi.yml
  format: yaml
  label: NICE Result API
  slug: nice-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-result-api-openapi.yml
- filename: nice-segments-api-openapi.yml
  format: yaml
  label: NICE Segments API
  slug: nice-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-segments-api-openapi.yml
- filename: nice-status-api-openapi.yml
  format: yaml
  label: NICE Status API
  slug: nice-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-status-api-openapi.yml
- filename: nice-user-management-api-openapi.yml
  format: yaml
  label: NICE User Management API
  slug: nice-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-user-management-api-openapi.yml
- filename: nice-voice-print-status-api-openapi.yml
  format: yaml
  label: NICE Voice Print Status API
  slug: nice-voice-print-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-voice-print-status-api-openapi.yml
- filename: nice-well-known-api-openapi.yml
  format: yaml
  label: NICE .well Known API
  slug: nice-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nice.com
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: www.nice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NICE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NICE
provider_slug: nice
slug: nice-domain-security
source_filename: nice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/security/nice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Customer Experience
- Artificial Intelligence
- Cloud
- Integration
---
