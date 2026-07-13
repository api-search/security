---
api_specs:
- filename: tanium-platform-rest-api-openapi.yml
  format: yaml
  label: Tanium Platform REST API
  slug: platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-platform-rest-api-openapi.yml
- filename: tanium-threat-response-api-openapi.yml
  format: yaml
  label: Tanium Threat Response API
  slug: threat-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-threat-response-api-openapi.yml
- filename: tanium-connect-api-openapi.yml
  format: yaml
  label: Tanium Connect API
  slug: connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-connect-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tanium.com
  spf: true
hosts:
- cert_expires: Sep 24 05:16:46 2026 GMT
  host: developer.tanium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.tanium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.tanium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tanium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tanium, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tanium
provider_slug: tanium
slug: tanium-domain-security
source_filename: tanium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tanium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:16:46 2026 GMT\n  hsts: false\n- host: www.tanium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: docs.tanium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tanium.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/security/tanium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
---
