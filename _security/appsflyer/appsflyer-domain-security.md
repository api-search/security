---
api_specs:
- filename: appsflyer-raw-data-pull-api-v2-token-openapi.yml
  format: yaml
  label: Pull API (Reporting Data)
  slug: pull-api-reporting-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-raw-data-pull-api-v2-token-openapi.yml
- filename: appsflyer-server-to-server-events-api-for-mobile-openapi.yml
  format: yaml
  label: Events APIs (Server-to-Server & Client-to-Server)
  slug: events-apis-server-to-server-client-to-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-server-to-server-events-api-for-mobile-openapi.yml
- filename: appsflyer-app-management-api-v20-openapi.yml
  format: yaml
  label: Management APIs
  slug: management-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-app-management-api-v20-openapi.yml
- filename: appsflyer-audience-external-api-openapi.yml
  format: yaml
  label: Audience APIs
  slug: audience-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-audience-external-api-openapi.yml
- filename: appsflyer-onelink-api-v20-openapi.yml
  format: yaml
  label: OneLink API
  slug: onelink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-onelink-api-v20-openapi.yml
- filename: appsflyer-skan-aggregated-performance-report-api-openapi.yml
  format: yaml
  label: SKAdNetwork (SKAN) APIs
  slug: skadnetwork-skan-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-skan-aggregated-performance-report-api-openapi.yml
- filename: appsflyer-opendsr-api-openapi.yml
  format: yaml
  label: OpenDSR API
  slug: opendsr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-opendsr-api-openapi.yml
- filename: appsflyer-click-signing-api-openapi.yml
  format: yaml
  label: Click Signing API (Protect360)
  slug: click-signing-api-protect360
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-click-signing-api-openapi.yml
- filename: appsflyer-roi360-net-revenue-api-v20-openapi.yml
  format: yaml
  label: ROI360 Net Revenue API
  slug: roi360-net-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-roi360-net-revenue-api-v20-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appsflyer.com
  spf: true
hosts:
- cert_expires: Oct 12 09:34:25 2026 GMT
  host: www.appsflyer.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:54:40 2026 GMT
  host: dev.appsflyer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: hq1.appsflyer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appsflyer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppsFlyer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppsFlyer
provider_slug: appsflyer
slug: appsflyer-domain-security
source_filename: appsflyer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appsflyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 09:34:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: dev.appsflyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:54:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hq1.appsflyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: appsflyer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/security/appsflyer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile Attribution
- Marketing Analytics
- Mobile Measurement
- Deep Linking
- Audiences
- Ad Fraud Prevention
- SKAdNetwork
- Privacy
- Advertising Technology
- Mobile SDK
- Agentic AI
---
