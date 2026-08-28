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
certifications:
- read_from_source
- claims
- note
description: ''
kind: trust-center
layout: security
name: Pypestream Trust Center
name_suffix: Trust Center
overview: Pypestream maintains a public trust center documenting read_from_source, claims, and note compliance.
provider_name: Pypestream
provider_slug: pypestream
slug: pypestream-trust-center
source_filename: pypestream-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://trust.pypestream.com/ (HTTP 200, probed 2026-08-26), https://www.pypestream.ai/security,\n  and the SSR meta of https://www.pypestream.ai/\ntrust_center:\n  url: https://trust.pypestream.com/\n  http_status: 200\n  vendor: Vanta\n  vendor_evidence: >-\n    Page title \"Pypestream Trust Center\"; the document loads only assets.vanta.com bundles\n    (index-trust-report-*.js, alpaca-*.js) and links a Vanta-hosted document at\n    app.vanta.com/doc?s=mfierwpbr76esz2ac3kgcg.\n  machine_readable: false\n  machine_readable_note: >-\n    The trust center is a client-rendered Vanta application. The HTML delivered to a non-JS client\n    is a 5.8KB shell containing the page title and nothing else -- no certification list, no\n    document index, no framework names. https://api.vanta.com/v1/trust-pages/pypestream returns 401.\n    The certifications Pypestream holds are therefore unreadable by any agent that does not execute\n\
  \    JavaScript, which is the finding: the trust center exists and is not machine-readable.\ncertifications:\n  read_from_source: false\n  claims:\n  - name: SOC 2\n    status: claimed\n    evidence: >-\n      \"SOC 2 certified.\" appears in the meta name=\"description\", og:description and\n      twitter:description of every document served by www.pypestream.ai. This is Pypestream's own\n      first-party assertion in its own markup.\n    source: https://www.pypestream.ai/\n    verified_against_report: false\n  note: >-\n    Only SOC 2 could be read first-party. The /security page is documented in Pypestream's own\n    sitemap.xml but the site is a single-page application that returns the identical 375,818-byte\n    homepage document, canonical https://www.pypestream.ai/, for every route -- so its content was\n    not machine-readable and no further certification is asserted here. Any additional framework\n    Pypestream holds is real but unrecorded, not absent; a JS-capable read of\n\
  \    https://trust.pypestream.com/ would resolve it.\nsecurity_page:\n  url: https://www.pypestream.ai/security\n  http_status: 200\n  readable: false\n  note: SPA route; serves the homepage shell to a non-JS client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/security/pypestream-trust-center.yml
summary_line: read_from_source, claims, note
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
trust_url: ''
---
