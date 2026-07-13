---
api_specs:
- filename: at-t-developer-hub-network-insights-api.yaml
  format: yaml
  label: AT&T Network Insights API
  slug: att-network-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-network-insights-api.yaml
- filename: at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
  format: yaml
  label: AT&T Mobility Threat and Anomaly Detection API
  slug: att-mobility-threat-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
- filename: at-t-developer-hub-sim-swap-api.yaml
  format: yaml
  label: AT&T SIM Swap API
  slug: att-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-sim-swap-api.yaml
- filename: at-t-developer-hub-device-status-api.yaml
  format: yaml
  label: AT&T Device Status API
  slug: att-device-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-device-status-api.yaml
- filename: at-t-developer-hub-quality-on-demand-api.yaml
  format: yaml
  label: AT&T Quality on Demand API
  slug: att-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-quality-on-demand-api.yaml
- filename: at-t-developer-hub-number-verification-api.yaml
  format: yaml
  label: AT&T Number Verification API
  slug: att-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-number-verification-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: att.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.att.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: developer.att.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: devex-web.att.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: At T Developer Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AT&T Developer Hub, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
slug: at-t-developer-hub-domain-security
source_filename: at-t-developer-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: devex-web.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: att.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/security/at-t-developer-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
---
