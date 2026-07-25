---
api_specs:
- filename: microsoft-power-bi-apps-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Apps API
  slug: microsoft-power-bi-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-apps-api-openapi.yml
- filename: microsoft-power-bi-capacities-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Capacities API
  slug: microsoft-power-bi-capacities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-capacities-api-openapi.yml
- filename: microsoft-power-bi-dashboards-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Dashboards API
  slug: microsoft-power-bi-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-dashboards-api-openapi.yml
- filename: microsoft-power-bi-dataflows-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Dataflows API
  slug: microsoft-power-bi-dataflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-dataflows-api-openapi.yml
- filename: microsoft-power-bi-datasets-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Datasets API
  slug: microsoft-power-bi-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-datasets-api-openapi.yml
- filename: microsoft-power-bi-embedtoken-api-openapi.yml
  format: yaml
  label: Microsoft Power BI EmbedToken API
  slug: microsoft-power-bi-embedtoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-embedtoken-api-openapi.yml
- filename: microsoft-power-bi-gateways-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Gateways API
  slug: microsoft-power-bi-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-gateways-api-openapi.yml
- filename: microsoft-power-bi-groups-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Groups API
  slug: microsoft-power-bi-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-groups-api-openapi.yml
- filename: microsoft-power-bi-imports-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Imports API
  slug: microsoft-power-bi-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-imports-api-openapi.yml
- filename: microsoft-power-bi-reports-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Reports API
  slug: microsoft-power-bi-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-reports-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: powerbi.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 16 16:30:49 2026 GMT
  host: app.powerbi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 22:02:24 2026 GMT
  host: powerbi.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Power Bi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Power BI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Power BI
provider_slug: microsoft-power-bi
slug: microsoft-power-bi-domain-security
source_filename: microsoft-power-bi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.powerbi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 16:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: powerbi.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 22:02:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powerbi.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/security/microsoft-power-bi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Microsoft
- Reports
---
