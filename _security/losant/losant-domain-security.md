---
api_specs:
- filename: losant-auth-api-openapi.yml
  format: yaml
  label: Losant Authentication And Account API
  slug: losant-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-auth-api-openapi.yml
- filename: losant-application-api-openapi.yml
  format: yaml
  label: Losant Application API
  slug: losant-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-application-api-openapi.yml
- filename: losant-device-api-openapi.yml
  format: yaml
  label: Losant Device API
  slug: losant-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-device-api-openapi.yml
- filename: losant-data-api-openapi.yml
  format: yaml
  label: Losant Data And Data Tables API
  slug: losant-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-data-api-openapi.yml
- filename: losant-workflow-api-openapi.yml
  format: yaml
  label: Losant Workflow Engine API
  slug: losant-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-workflow-api-openapi.yml
- filename: losant-edge-api-openapi.yml
  format: yaml
  label: Losant Edge And Embedded Compute API
  slug: losant-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-edge-api-openapi.yml
- filename: losant-experience-api-openapi.yml
  format: yaml
  label: Losant Experience API
  slug: losant-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-experience-api-openapi.yml
- filename: losant-notebook-api-openapi.yml
  format: yaml
  label: Losant Notebooks API
  slug: losant-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-notebook-api-openapi.yml
- filename: losant-instance-api-openapi.yml
  format: yaml
  label: Losant Enterprise Instance API
  slug: losant-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-instance-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: losant.com
  spf: true
hosts:
- cert_expires: Sep 28 23:00:49 2026 GMT
  host: www.losant.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:59:59 2026 GMT
  host: docs.losant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:59:59 2026 GMT
  host: api.losant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Losant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Losant, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Losant
provider_slug: losant
slug: losant-domain-security
source_filename: losant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.losant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: docs.losant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.losant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: losant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/security/losant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Internet Of Things
- Devices
- Edge Compute
- Embedded
- MQTT
- Industrial IoT
- Telemetry
- Workflow Automation
- Visual Workflow Engine
- Dashboards
- Time Series
- Connected Products
- Enterprise
---
