---
api_specs:
- filename: tealium-collect-http-openapi.yml
  format: yaml
  label: Tealium Collect HTTP API
  slug: tealium-collect-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-collect-http-openapi.yml
- filename: tealium-visitor-profile-openapi.yml
  format: yaml
  label: Tealium Visitor Profile API
  slug: tealium-visitor-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-visitor-profile-openapi.yml
- filename: tealium-visitor-privacy-openapi.yml
  format: yaml
  label: Tealium Visitor Privacy API
  slug: tealium-visitor-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-visitor-privacy-openapi.yml
- filename: tealium-moments-openapi.yml
  format: yaml
  label: Tealium Moments API
  slug: tealium-moments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-moments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tealium.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tealiumapis.com
  spf: false
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: tealium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 08:45:19 2026 GMT
  host: docs.tealium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: platform.tealiumapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tealium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tealium, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tealium
provider_slug: tealium
slug: tealium-domain-security
source_filename: tealium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tealium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tealium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:45:19 2026 GMT\n  hsts: false\n- host: platform.tealiumapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tealium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tealiumapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/security/tealium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- CDP
- Tag Management
- AudienceStream
- Real-Time Events
- Visitor Profiles
- Audience Segmentation
- Data Collection
- Privacy Compliance
- Personalization
---
