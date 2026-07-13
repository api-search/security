---
api_specs:
- filename: orange-business-number-verification-openapi.yml
  format: yaml
  label: Orange Business Number Verification API
  slug: orange-business-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-number-verification-openapi.yml
- filename: orange-business-sim-swap-openapi.yml
  format: yaml
  label: Orange Business SIM Swap API
  slug: orange-business-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-sim-swap-openapi.yml
- filename: orange-business-device-swap-openapi.yml
  format: yaml
  label: Orange Business Device Swap API
  slug: orange-business-device-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-swap-openapi.yml
- filename: orange-business-kyc-match-openapi.yml
  format: yaml
  label: Orange Business KYC Match API
  slug: orange-business-kyc-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-kyc-match-openapi.yml
- filename: orange-business-device-location-retrieval-openapi.yml
  format: yaml
  label: Orange Business Device Location Retrieval API
  slug: orange-business-device-location-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-location-retrieval-openapi.yml
- filename: orange-business-device-location-verification-openapi.yml
  format: yaml
  label: Orange Business Device Location Verification API
  slug: orange-business-device-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-location-verification-openapi.yml
- filename: orange-business-geofencing-openapi.yml
  format: yaml
  label: Orange Business Geofencing API
  slug: orange-business-geofencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-geofencing-openapi.yml
- filename: orange-business-device-reachability-status-openapi.yml
  format: yaml
  label: Orange Business Device Reachability Status API
  slug: orange-business-device-reachability-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-reachability-status-openapi.yml
- filename: orange-business-device-roaming-status-openapi.yml
  format: yaml
  label: Orange Business Device Roaming Status API
  slug: orange-business-device-roaming-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-roaming-status-openapi.yml
- filename: orange-business-quality-on-demand-openapi.yml
  format: yaml
  label: Orange Business Quality on Demand API
  slug: orange-business-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-quality-on-demand-openapi.yml
- filename: orange-business-population-density-data-openapi.yml
  format: yaml
  label: Orange Business Population Density Data API
  slug: orange-business-population-density-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-population-density-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: orange.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orange-business.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: developer.orange.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: www.orange-business.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: liveobjects.orange-business.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orange Business Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orange Business, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Orange Business
provider_slug: orange-business
slug: orange-business-domain-security
source_filename: orange-business-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.orange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.orange-business.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: liveobjects.orange-business.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orange.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: orange-business.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/security/orange-business-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- 5G
- AI
- B2B
- CAMARA
- Cloud
- Communications
- Cybersecurity
- Developer Platform
- Digital Workplace
- Enterprise
- France
- IoT
- Identity
- Mobile Money
- Network APIs
- Open Gateway
- Orange
- Payments
- SD-WAN
- SMS
- SASE
- Telco
- Voice
---
