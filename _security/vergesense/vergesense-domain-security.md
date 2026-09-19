---
api_specs:
- filename: vergesense-buildings-api-openapi.yml
  format: yaml
  label: VergeSense Buildings API
  slug: vergesense-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-buildings-api-openapi.yml
- filename: vergesense-hardware-api-openapi.yml
  format: yaml
  label: VergeSense Hardware API
  slug: vergesense-hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-hardware-api-openapi.yml
- filename: vergesense-metrics-api-openapi.yml
  format: yaml
  label: VergeSense Metrics API
  slug: vergesense-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-metrics-api-openapi.yml
- filename: vergesense-predict-api-openapi.yml
  format: yaml
  label: VergeSense Predict API
  slug: vergesense-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-predict-api-openapi.yml
- filename: vergesense-sensors-api-openapi.yml
  format: yaml
  label: VergeSense Sensors API
  slug: vergesense-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-sensors-api-openapi.yml
- filename: vergesense-spaces-api-openapi.yml
  format: yaml
  label: VergeSense Spaces API
  slug: vergesense-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-spaces-api-openapi.yml
- filename: vergesense-webhooks-api-openapi.yml
  format: yaml
  label: VergeSense Webhooks API
  slug: vergesense-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vergesense.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Nov 17 16:38:08 2026 GMT
  host: www.vergesense.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: vergesense.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 07:53:52 2026 GMT
  host: api.vergesense.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Vergesense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VergeSense, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: VergeSense
provider_slug: vergesense
slug: vergesense-domain-security
source_filename: vergesense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vergesense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 16:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vergesense.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vergesense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 07:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vergesense.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/security/vergesense-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Occupancy Intelligence
- Workplace Analytics
- Corporate Real Estate
- PropTech
- IoT Sensors
- Building Data
- Space Utilization
- Facilities Management
- Smart Buildings
- Webhook
- MCP
- JSON:API
---
