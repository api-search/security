---
api_specs:
- filename: swagger.json
  format: json
  label: Adobe Analytics API
  slug: adobe-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/AdobeDocs/analytics-2.0-apis/main/docs/swagger.json
- filename: adobe-analytics-bulk-data-insertion-api-openapi.yml
  format: yaml
  label: Adobe Analytics Bulk Data Insertion API
  slug: adobe-analytics-bulk-data-insertion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-bulk-data-insertion-api-openapi.yml
- filename: adobe-analytics-livestream-asyncapi.yml
  format: yaml
  label: Adobe Analytics Livestream API
  slug: adobe-analytics-livestream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/asyncapi/adobe-analytics-livestream-asyncapi.yml
- filename: adobe-analytics-data-repair-api-openapi.yml
  format: yaml
  label: Adobe Analytics Data Repair API
  slug: adobe-analytics-data-repair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-data-repair-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.io
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: analytics-collection.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: analytics-collection-us.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Analytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Analytics
provider_slug: adobe-analytics
slug: adobe-analytics-domain-security
source_filename: adobe-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: analytics-collection.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\n- host: analytics-collection-us.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/security/adobe-analytics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
---
