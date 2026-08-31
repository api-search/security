---
api_specs:
- filename: phosphorus-alerts-api-openapi.yml
  format: yaml
  label: Phosphorus Alerts API
  slug: phosphorus-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-alerts-api-openapi.yml
- filename: phosphorus-device-api-openapi.yml
  format: yaml
  label: Phosphorus Device API
  slug: phosphorus-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-device-api-openapi.yml
- filename: phosphorus-devices-api-openapi.yml
  format: yaml
  label: Phosphorus Devices API
  slug: phosphorus-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-devices-api-openapi.yml
- filename: phosphorus-dynamic-scans-api-openapi.yml
  format: yaml
  label: Phosphorus Dynamic Scans API
  slug: phosphorus-dynamic-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-dynamic-scans-api-openapi.yml
- filename: phosphorus-providers-api-openapi.yml
  format: yaml
  label: Phosphorus Providers API
  slug: phosphorus-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-providers-api-openapi.yml
- filename: phosphorus-search-api-openapi.yml
  format: yaml
  label: Phosphorus Search API
  slug: phosphorus-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-search-api-openapi.yml
- filename: phosphorus-sites-api-openapi.yml
  format: yaml
  label: Phosphorus Sites API
  slug: phosphorus-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-sites-api-openapi.yml
- filename: phosphorus-vault-api-openapi.yml
  format: yaml
  label: Phosphorus Vault API
  slug: phosphorus-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-vault-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: phosphorus.io
  spf: true
hosts:
- cert_expires: Nov 12 21:19:01 2026 GMT
  host: phosphorus.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phosphorus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phosphorus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Phosphorus
provider_slug: phosphorus
slug: phosphorus-domain-security
source_filename: phosphorus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phosphorus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 21:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: phosphorus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/security/phosphorus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- xIoT Security
- IoT Security
- OT Security
- IoMT
- Asset Discovery
- Vulnerability Management
- Firmware Management
- Certificate Management
- Credential Management
- Critical Infrastructure
- Device Management
---
