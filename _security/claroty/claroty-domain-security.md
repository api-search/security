---
api_specs:
- filename: claroty-authenticate-api-openapi.yml
  format: yaml
  label: Claroty Authenticate API
  slug: claroty-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-authenticate-api-openapi.yml
- filename: claroty-health-api-openapi.yml
  format: yaml
  label: Claroty Health API
  slug: claroty-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-health-api-openapi.yml
- filename: claroty-is-key-registered-api-openapi.yml
  format: yaml
  label: Claroty Is Key Registered API
  slug: claroty-is-key-registered-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-is-key-registered-api-openapi.yml
- filename: claroty-jwks-api-openapi.yml
  format: yaml
  label: Claroty Jwks API
  slug: claroty-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-jwks-api-openapi.yml
- filename: claroty-jwthenticator-api-openapi.yml
  format: yaml
  label: Claroty JW Thenticator API
  slug: claroty-jwthenticator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-jwthenticator-api-openapi.yml
- filename: claroty-refresh-api-openapi.yml
  format: yaml
  label: Claroty Refresh API
  slug: claroty-refresh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-refresh-api-openapi.yml
- filename: claroty-register-key-api-openapi.yml
  format: yaml
  label: Claroty Register Key API
  slug: claroty-register-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-register-key-api-openapi.yml
- filename: claroty-validate-api-openapi.yml
  format: yaml
  label: Claroty Validate API
  slug: claroty-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-validate-api-openapi.yml
- filename: claroty-validate-request-api-openapi.yml
  format: yaml
  label: Claroty Validate Request API
  slug: claroty-validate-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-validate-request-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: claroty.com
  spf: true
hosts:
- cert_expires: Nov  1 19:38:07 2026 GMT
  host: www.claroty.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claroty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claroty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Claroty
provider_slug: claroty
slug: claroty-domain-security
source_filename: claroty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.claroty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 19:38:07 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: claroty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/security/claroty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- OT Security
- Cyber-Physical Systems
- IoT Security
- Industrial Control Systems
- Threat Detection
- Exposure Management
- Healthcare Security
---
