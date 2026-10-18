---
api_specs:
- filename: adjust-cost-api-openapi.yml
  format: yaml
  label: Adjust Cost API
  slug: adjust-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/openapi/adjust-cost-api-openapi.yml
- filename: adjust-dashboard-api-openapi.yml
  format: yaml
  label: Adjust Dashboard API
  slug: adjust-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/openapi/adjust-dashboard-api-openapi.yml
- filename: adjust-device-service-api-openapi.yml
  format: yaml
  label: Adjust Device Service API
  slug: adjust-device-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/openapi/adjust-device-service-api-openapi.yml
- filename: adjust-public-api-openapi.yml
  format: yaml
  label: Adjust Public API
  slug: adjust-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/openapi/adjust-public-api-openapi.yml
- filename: adjust-reports-service-api-openapi.yml
  format: yaml
  label: Adjust Reports Service API
  slug: adjust-reports-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/openapi/adjust-reports-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adjust.com
  spf: true
hosts:
- cert_expires: Dec 19 01:00:08 2026 GMT
  host: www.adjust.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adjust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adjust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adjust
provider_slug: adjust
slug: adjust-domain-security
source_filename: adjust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adjust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:00:08 2026 GMT\n  hsts: null\ndomains:\n- domain: adjust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/security/adjust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Measurements
- Analytics
- Attribution
- Deep Linking
- Fraud Prevention
- Mobile Marketing
- AI Solutions
- Gaming
---
