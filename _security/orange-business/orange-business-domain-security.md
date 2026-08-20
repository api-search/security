---
api_specs:
- filename: orange-business-check-device-swap-api-openapi.yml
  format: yaml
  label: Orange Business Check Device Swap API
  slug: orange-business-check-device-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-check-device-swap-api-openapi.yml
- filename: orange-business-check-sim-swap-api-openapi.yml
  format: yaml
  label: Orange Business Check SIM swap API
  slug: orange-business-check-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-check-sim-swap-api-openapi.yml
- filename: orange-business-device-reachability-status-api-openapi.yml
  format: yaml
  label: Orange Business Device reachability status API
  slug: orange-business-device-reachability-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-reachability-status-api-openapi.yml
- filename: orange-business-geofencing-subscriptions-api-openapi.yml
  format: yaml
  label: Orange Business Geofencing subscriptions API
  slug: orange-business-geofencing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-geofencing-subscriptions-api-openapi.yml
- filename: orange-business-location-retrieval-api-openapi.yml
  format: yaml
  label: Orange Business Location retrieval API
  slug: orange-business-location-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-location-retrieval-api-openapi.yml
- filename: orange-business-location-verification-api-openapi.yml
  format: yaml
  label: Orange Business Location verification API
  slug: orange-business-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-location-verification-api-openapi.yml
- filename: orange-business-match-api-openapi.yml
  format: yaml
  label: Orange Business Match API
  slug: orange-business-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-match-api-openapi.yml
- filename: orange-business-phone-number-share-api-openapi.yml
  format: yaml
  label: Orange Business Phone number share API
  slug: orange-business-phone-number-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-phone-number-share-api-openapi.yml
- filename: orange-business-phone-number-verify-api-openapi.yml
  format: yaml
  label: Orange Business Phone number verify API
  slug: orange-business-phone-number-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-phone-number-verify-api-openapi.yml
- filename: orange-business-population-density-data-api-openapi.yml
  format: yaml
  label: Orange Business Population Density Data API
  slug: orange-business-population-density-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-population-density-data-api-openapi.yml
- filename: orange-business-qos-sessions-api-openapi.yml
  format: yaml
  label: Orange Business QoS Sessions API
  slug: orange-business-qos-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-qos-sessions-api-openapi.yml
- filename: orange-business-retrieve-device-swap-date-api-openapi.yml
  format: yaml
  label: Orange Business Retrieve Device Swap Date API
  slug: orange-business-retrieve-device-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-retrieve-device-swap-date-api-openapi.yml
- filename: orange-business-retrieve-sim-swap-date-api-openapi.yml
  format: yaml
  label: Orange Business Retrieve SIM swap date API
  slug: orange-business-retrieve-sim-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-retrieve-sim-swap-date-api-openapi.yml
- filename: orange-business-roaming-status-retrieval-api-openapi.yml
  format: yaml
  label: Orange Business Roaming status retrieval API
  slug: orange-business-roaming-status-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-roaming-status-retrieval-api-openapi.yml
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
- Artificial Intelligence
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
