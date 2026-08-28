---
api_specs:
- filename: pypestream-reporting-api-openapi.json
  format: json
  label: Pypestream Reporting API
  slug: reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-reporting-api-openapi.json
- filename: pypestream-contact-center-api-openapi.json
  format: json
  label: Pypestream Contact Center API
  slug: contact-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-contact-center-api-openapi.json
- filename: pypestream-middleware-api-openapi.json
  format: json
  label: Pypestream Middleware API
  slug: middleware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-middleware-api-openapi.json
- filename: pypestream-engagement-api-openapi.json
  format: json
  label: Pypestream Engagement API
  slug: engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-engagement-api-openapi.json
- filename: pypestream-analytics-api-openapi.json
  format: json
  label: Pypestream Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-analytics-api-openapi.json
- filename: pypestream-javascript-sdk-openapi.json
  format: json
  label: Pypestream JavaScript SDK API
  slug: javascript-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-javascript-sdk-openapi.json
- filename: pypestream-insights-api-openapi.json
  format: json
  label: Pypestream Insights API
  slug: insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-insights-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pypestream.ai
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pypestream.com
  spf: true
hosts:
- cert_expires: Nov 22 04:50:16 2026 GMT
  host: www.pypestream.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 03:56:55 2026 GMT
  host: developers.pypestream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: reporting.pypestream.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pypestream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pypestream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pypestream
provider_slug: pypestream
slug: pypestream-domain-security
source_filename: pypestream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pypestream.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 04:50:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.pypestream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 03:56:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: reporting.pypestream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pypestream.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: pypestream.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/security/pypestream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Conversational AI
- Agentic AI
- Contact Center
- Customer Service
- Customer Engagement
- Chatbots
- Voice AI
- Messaging
- Analytics
- Enterprise Software
---
