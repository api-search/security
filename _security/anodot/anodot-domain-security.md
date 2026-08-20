---
api_specs:
- filename: anodot-access-token-api-openapi.yml
  format: yaml
  label: Anodot Access Token API
  slug: anodot-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-access-token-api-openapi.yml
- filename: anodot-alert-actions-api-openapi.yml
  format: yaml
  label: Anodot Alert Actions API
  slug: anodot-alert-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-alert-actions-api-openapi.yml
- filename: anodot-alerts-api-openapi.yml
  format: yaml
  label: Anodot Alerts API
  slug: anodot-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-alerts-api-openapi.yml
- filename: anodot-anomalies-api-openapi.yml
  format: yaml
  label: Anodot Anomalies API
  slug: anodot-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-anomalies-api-openapi.yml
- filename: anodot-customers-api-openapi.yml
  format: yaml
  label: Anodot Customers API
  slug: anodot-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-customers-api-openapi.yml
- filename: anodot-forecast-api-openapi.yml
  format: yaml
  label: Anodot Forecast API
  slug: anodot-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-forecast-api-openapi.yml
- filename: anodot-groups-api-openapi.yml
  format: yaml
  label: Anodot Groups API
  slug: anodot-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-groups-api-openapi.yml
- filename: anodot-users-api-openapi.yml
  format: yaml
  label: Anodot Users API
  slug: anodot-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anodot.com
  spf: true
hosts:
- cert_expires: Sep 14 07:42:38 2026 GMT
  host: www.anodot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: cloudcost.anodot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: docs.anodot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anodot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anodot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anodot
provider_slug: anodot
slug: anodot-domain-security
source_filename: anodot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anodot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:42:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloudcost.anodot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.anodot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: anodot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/security/anodot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Anomaly Detection
- Business Monitoring
- Cloud Cost Management
- FinOps
- Machine-Learning
- Observability
---
