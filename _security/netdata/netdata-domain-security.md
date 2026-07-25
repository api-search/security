---
api_specs:
- filename: netdata-swagger.yaml
  format: yaml
  label: Netdata Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/netdata/netdata/master/src/web/api/netdata-swagger.yaml
- filename: netdata-alerts-api-openapi.yml
  format: yaml
  label: Netdata alerts API
  slug: netdata-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-alerts-api-openapi.yml
- filename: netdata-authentication-api-openapi.yml
  format: yaml
  label: Netdata authentication API
  slug: netdata-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-authentication-api-openapi.yml
- filename: netdata-badges-api-openapi.yml
  format: yaml
  label: Netdata badges API
  slug: netdata-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-badges-api-openapi.yml
- filename: netdata-charts-api-openapi.yml
  format: yaml
  label: Netdata charts API
  slug: netdata-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-charts-api-openapi.yml
- filename: netdata-claiming-api-openapi.yml
  format: yaml
  label: Netdata claiming API
  slug: netdata-claiming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-claiming-api-openapi.yml
- filename: netdata-config-api-openapi.yml
  format: yaml
  label: Netdata config API
  slug: netdata-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-config-api-openapi.yml
- filename: netdata-contexts-api-openapi.yml
  format: yaml
  label: Netdata contexts API
  slug: netdata-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-contexts-api-openapi.yml
- filename: netdata-data-api-openapi.yml
  format: yaml
  label: Netdata data API
  slug: netdata-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-data-api-openapi.yml
- filename: netdata-dyncfg-api-openapi.yml
  format: yaml
  label: Netdata dyncfg API
  slug: netdata-dyncfg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-dyncfg-api-openapi.yml
- filename: netdata-functions-api-openapi.yml
  format: yaml
  label: Netdata functions API
  slug: netdata-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-functions-api-openapi.yml
- filename: netdata-management-api-openapi.yml
  format: yaml
  label: Netdata management API
  slug: netdata-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-management-api-openapi.yml
- filename: netdata-nodes-api-openapi.yml
  format: yaml
  label: Netdata nodes API
  slug: netdata-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-nodes-api-openapi.yml
- filename: netdata-registry-api-openapi.yml
  format: yaml
  label: Netdata registry API
  slug: netdata-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-registry-api-openapi.yml
- filename: netdata-settings-api-openapi.yml
  format: yaml
  label: Netdata settings API
  slug: netdata-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-settings-api-openapi.yml
- filename: netdata-streaming-api-openapi.yml
  format: yaml
  label: Netdata streaming API
  slug: netdata-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-streaming-api-openapi.yml
- filename: netdata-variables-api-openapi.yml
  format: yaml
  label: Netdata variables API
  slug: netdata-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-variables-api-openapi.yml
- filename: netdata-versions-api-openapi.yml
  format: yaml
  label: Netdata versions API
  slug: netdata-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-versions-api-openapi.yml
- filename: netdata-webrtc-api-openapi.yml
  format: yaml
  label: Netdata webrtc API
  slug: netdata-webrtc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-webrtc-api-openapi.yml
- filename: netdata-weights-api-openapi.yml
  format: yaml
  label: Netdata weights API
  slug: netdata-weights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-weights-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: netdata.cloud
  spf: true
hosts:
- cert_expires: Oct  2 19:18:18 2026 GMT
  host: www.netdata.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:07:14 2026 GMT
  host: learn.netdata.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 18:05:47 2026 GMT
  host: app.netdata.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netdata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Netdata
provider_slug: netdata
slug: netdata-domain-security
source_filename: netdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:18:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.netdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:07:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.netdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:05:47 2026 GMT\n  hsts: false\ndomains:\n- domain: netdata.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/security/netdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monitoring
- Observability
- Infrastructure
- Metrics
- Alerts
- Real-Time
- APM
- DevOps
---
