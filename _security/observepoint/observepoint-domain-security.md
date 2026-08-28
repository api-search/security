---
api_specs:
- filename: observepoint-v3-api-openapi.yml
  format: yaml
  label: ObservePoint V3 API
  slug: observepoint-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/openapi/observepoint-v3-api-openapi.yml
- filename: observepoint-grid-reports-api-openapi.yml
  format: yaml
  label: ObservePoint Grid Reporting API
  slug: observepoint-grid-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/openapi/observepoint-grid-reports-api-openapi.yml
- filename: observepoint-v2-api-openapi.yml
  format: yaml
  label: ObservePoint V2 API
  slug: observepoint-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/openapi/observepoint-v2-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "starfieldtech.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: observepoint.com
  spf: true
hosts:
- cert_expires: Oct  7 09:35:00 2026 GMT
  host: www.observepoint.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 20:02:48 2026 GMT
  host: api-docs.observepoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.observepoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Observepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ObservePoint, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ObservePoint
provider_slug: observepoint
slug: observepoint-domain-security
source_filename: observepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.observepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:35:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api-docs.observepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 20:02:48 2026 GMT\n  hsts: false\n- host: api.observepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: observepoint.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/observepoint/refs/heads/main/security/observepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web Governance
- Tag Management
- Analytics Validation
- Privacy Compliance
- Consent Management
- Web Accessibility
- Data Quality
- Marketing Technology
- Website Auditing
- Digital Analytics
- Webhooks
---
