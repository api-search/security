---
api_specs:
- filename: adobe-analytics-livestream-asyncapi.yml
  format: yaml
  label: Adobe Analytics Livestream API
  slug: adobe-analytics-livestream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/asyncapi/adobe-analytics-livestream-asyncapi.yml
- filename: adobe-analytics-annotations-api-openapi.yml
  format: yaml
  label: Adobe Analytics Annotations API
  slug: adobe-analytics-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-annotations-api-openapi.yml
- filename: adobe-analytics-calculated-metrics-api-openapi.yml
  format: yaml
  label: Adobe Analytics Calculated Metrics API
  slug: adobe-analytics-calculated-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-calculated-metrics-api-openapi.yml
- filename: adobe-analytics-date-ranges-api-openapi.yml
  format: yaml
  label: Adobe Analytics Date Ranges API
  slug: adobe-analytics-date-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-date-ranges-api-openapi.yml
- filename: adobe-analytics-dimensions-api-openapi.yml
  format: yaml
  label: Adobe Analytics Dimensions API
  slug: adobe-analytics-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-dimensions-api-openapi.yml
- filename: adobe-analytics-events-api-openapi.yml
  format: yaml
  label: Adobe Analytics Events API
  slug: adobe-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-events-api-openapi.yml
- filename: adobe-analytics-jobs-api-openapi.yml
  format: yaml
  label: Adobe Analytics Jobs API
  slug: adobe-analytics-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-jobs-api-openapi.yml
- filename: adobe-analytics-metrics-api-openapi.yml
  format: yaml
  label: Adobe Analytics Metrics API
  slug: adobe-analytics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-metrics-api-openapi.yml
- filename: adobe-analytics-report-suites-api-openapi.yml
  format: yaml
  label: Adobe Analytics Report Suites API
  slug: adobe-analytics-report-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-report-suites-api-openapi.yml
- filename: adobe-analytics-reports-api-openapi.yml
  format: yaml
  label: Adobe Analytics Reports API
  slug: adobe-analytics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-reports-api-openapi.yml
- filename: adobe-analytics-segments-api-openapi.yml
  format: yaml
  label: Adobe Analytics Segments API
  slug: adobe-analytics-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-segments-api-openapi.yml
- filename: adobe-analytics-server-call-estimate-api-openapi.yml
  format: yaml
  label: Adobe Analytics Server Call Estimate API
  slug: adobe-analytics-server-call-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-server-call-estimate-api-openapi.yml
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
