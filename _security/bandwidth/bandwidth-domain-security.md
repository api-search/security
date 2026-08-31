---
api_specs:
- filename: bandwidth-calls-api-openapi.yml
  format: yaml
  label: Bandwidth Calls API
  slug: bandwidth-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-calls-api-openapi.yml
- filename: bandwidth-conferences-api-openapi.yml
  format: yaml
  label: Bandwidth Conferences API
  slug: bandwidth-conferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-conferences-api-openapi.yml
- filename: bandwidth-emergency-notification-recipients-api-openapi.yml
  format: yaml
  label: Bandwidth Emergency Notification Recipients API
  slug: bandwidth-emergency-notification-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-emergency-notification-recipients-api-openapi.yml
- filename: bandwidth-endpoints-api-openapi.yml
  format: yaml
  label: Bandwidth Endpoints API
  slug: bandwidth-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-endpoints-api-openapi.yml
- filename: bandwidth-locations-api-openapi.yml
  format: yaml
  label: Bandwidth Locations API
  slug: bandwidth-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-locations-api-openapi.yml
- filename: bandwidth-media-api-openapi.yml
  format: yaml
  label: Bandwidth Media API
  slug: bandwidth-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-media-api-openapi.yml
- filename: bandwidth-messages-api-openapi.yml
  format: yaml
  label: Bandwidth Messages API
  slug: bandwidth-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-messages-api-openapi.yml
- filename: bandwidth-recordings-api-openapi.yml
  format: yaml
  label: Bandwidth Recordings API
  slug: bandwidth-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-recordings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bandwidth.com
  spf: true
hosts:
- cert_expires: Sep 27 03:11:29 2026 GMT
  host: www.bandwidth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: dev.bandwidth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 16:47:28 2026 GMT
  host: voice.bandwidth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bandwidth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bandwidth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bandwidth
provider_slug: bandwidth
slug: bandwidth-domain-security
source_filename: bandwidth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bandwidth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.bandwidth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: voice.bandwidth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:47:28 2026 GMT\n  hsts: null\ndomains:\n- domain: bandwidth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/security/bandwidth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
---
