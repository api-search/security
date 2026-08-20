---
api_specs:
- filename: zaius-compliance-api-openapi.yml
  format: yaml
  label: Zaius Compliance API
  slug: zaius-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-compliance-api-openapi.yml
- filename: zaius-consent-api-openapi.yml
  format: yaml
  label: Zaius Consent API
  slug: zaius-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-consent-api-openapi.yml
- filename: zaius-consent-legacy-api-openapi.yml
  format: yaml
  label: Zaius Consent (Legacy) API
  slug: zaius-consent-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-consent-legacy-api-openapi.yml
- filename: zaius-customers-api-openapi.yml
  format: yaml
  label: Zaius Customers API
  slug: zaius-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-customers-api-openapi.yml
- filename: zaius-events-api-openapi.yml
  format: yaml
  label: Zaius Events API
  slug: zaius-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-events-api-openapi.yml
- filename: zaius-exports-api-openapi.yml
  format: yaml
  label: Zaius Exports API
  slug: zaius-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-exports-api-openapi.yml
- filename: zaius-fields-schema-api-openapi.yml
  format: yaml
  label: Zaius Fields schema API
  slug: zaius-fields-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-fields-schema-api-openapi.yml
- filename: zaius-identifiers-api-openapi.yml
  format: yaml
  label: Zaius Identifiers API
  slug: zaius-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-identifiers-api-openapi.yml
- filename: zaius-lists-api-openapi.yml
  format: yaml
  label: Zaius Lists API
  slug: zaius-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-lists-api-openapi.yml
- filename: zaius-object-schema-api-openapi.yml
  format: yaml
  label: Zaius Object schema API
  slug: zaius-object-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-object-schema-api-openapi.yml
- filename: zaius-objects-api-openapi.yml
  format: yaml
  label: Zaius Objects API
  slug: zaius-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-objects-api-openapi.yml
- filename: zaius-orders-api-openapi.yml
  format: yaml
  label: Zaius Orders API
  slug: zaius-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-orders-api-openapi.yml
- filename: zaius-products-api-openapi.yml
  format: yaml
  label: Zaius Products API
  slug: zaius-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-products-api-openapi.yml
- filename: zaius-reachability-api-openapi.yml
  format: yaml
  label: Zaius Reachability API
  slug: zaius-reachability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-reachability-api-openapi.yml
- filename: zaius-realtimesegments-api-openapi.yml
  format: yaml
  label: Zaius RealtimeSegments API
  slug: zaius-realtimesegments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-realtimesegments-api-openapi.yml
- filename: zaius-recommendations-api-openapi.yml
  format: yaml
  label: Zaius Recommendations API
  slug: zaius-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-recommendations-api-openapi.yml
- filename: zaius-relationships-schema-api-openapi.yml
  format: yaml
  label: Zaius Relationships schema API
  slug: zaius-relationships-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-relationships-schema-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zaius.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optimizely.com
  spf: true
hosts:
- cert_expires: Sep  3 22:33:20 2026 GMT
  host: www.zaius.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.us1.odp.optimizely.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: api.eu1.odp.optimizely.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zaius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zaius, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zaius
provider_slug: zaius
slug: zaius-domain-security
source_filename: zaius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zaius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 22:33:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us1.odp.optimizely.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\n- host: api.eu1.odp.optimizely.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zaius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: optimizely.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/security/zaius-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Customer Data Platform
- CDP
- Marketing
- Personalization
- Segmentation
- E-Commerce
- Customer Data
- Real-Time Audiences
- Event
---
