---
api_specs:
- filename: sensors-data-analytics-channel-v1-openapi.yml
  format: yaml
  label: Sensors Analytics OpenAPI (神策分析)
  slug: sensors-analytics-openapi-神策分析
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-analytics-channel-v1-openapi.yml
- filename: sensors-data-horizon-catalog-v1-openapi.yml
  format: yaml
  label: Sensors Horizon CDP OpenAPI (神策数界)
  slug: sensors-horizon-cdp-openapi-神策数界
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-horizon-catalog-v1-openapi.yml
- filename: sensors-data-focus-express-action-channel-v1-openapi.yml
  format: yaml
  label: Sensors Focus OpenAPI (神策智能运营)
  slug: sensors-focus-openapi-神策智能运营
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-focus-express-action-channel-v1-openapi.yml
- filename: sensors-data-portal-identity-v2-openapi.yml
  format: yaml
  label: Sensors Portal OpenAPI (神策业务门户)
  slug: sensors-portal-openapi-神策业务门户
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-portal-identity-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sensorsdata.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: sensorsdata.cn
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.sensorsdata.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  5 18:02:41 2026 GMT
  host: docs.sensorsdata.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: manual.sensorsdata.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensors Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensors Data, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sensors Data
provider_slug: sensors-data
slug: sensors-data-domain-security
source_filename: sensors-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sensorsdata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\n- host: docs.sensorsdata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 18:02:41 2026 GMT\n  hsts: false\n- host: manual.sensorsdata.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sensorsdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: sensorsdata.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/security/sensors-data-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Enterprise
- Analytics
- Customer Data Platform
- Product Analytics
- Data Collection
- SDK
- Marketing
---
