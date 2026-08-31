---
api_specs:
- filename: losant-authentication-and-account-api-openapi.yml
  format: yaml
  label: Losant Authentication and Account API
  slug: losant-authentication-and-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-authentication-and-account-api-openapi.yml
- filename: losant-data-and-data-tables-api-openapi.yml
  format: yaml
  label: Losant Data and Data Tables API
  slug: losant-data-and-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-data-and-data-tables-api-openapi.yml
- filename: losant-edge-and-embedded-compute-api-openapi.yml
  format: yaml
  label: Losant Edge and Embedded Compute API
  slug: losant-edge-and-embedded-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-edge-and-embedded-compute-api-openapi.yml
- filename: losant-enterprise-instance-api-openapi.yml
  format: yaml
  label: Losant Enterprise Instance API
  slug: losant-enterprise-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-enterprise-instance-api-openapi.yml
- filename: losant-notebooks-api-openapi.yml
  format: yaml
  label: Losant Notebooks API
  slug: losant-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-notebooks-api-openapi.yml
- filename: losant-workflow-engine-api-openapi.yml
  format: yaml
  label: Losant Workflow Engine API
  slug: losant-workflow-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-workflow-engine-api-openapi.yml
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
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: docs.losant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
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
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.losant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: docs.losant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: false\n- host: api.losant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: losant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
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
- Workflow-Automation
- Visual Workflow Engine
- Dashboards
- Time Series
- Connected Products
- Enterprise
---
