---
api_specs:
- filename: tealium-auth-api-openapi.yml
  format: yaml
  label: Tealium Auth API
  slug: tealium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-auth-api-openapi.yml
- filename: tealium-collect-api-openapi.yml
  format: yaml
  label: Tealium Collect API
  slug: tealium-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-collect-api-openapi.yml
- filename: tealium-customer-api-openapi.yml
  format: yaml
  label: Tealium Customer API
  slug: tealium-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-customer-api-openapi.yml
- filename: tealium-personalization-api-openapi.yml
  format: yaml
  label: Tealium Personalization API
  slug: tealium-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-personalization-api-openapi.yml
- filename: tealium-privacy-api-openapi.yml
  format: yaml
  label: Tealium Privacy API
  slug: tealium-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-privacy-api-openapi.yml
- filename: tealium-ai-read-openapi.yml
  format: yaml
  label: Tealium AI Read API
  slug: tealium-ai-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-ai-read-openapi.yml
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
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tealium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tealium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:45:19 2026 GMT\n  hsts: false\n- host: platform.tealiumapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tealium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tealiumapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
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
