---
api_specs:
- filename: niural-authentication-api-openapi.yml
  format: yaml
  label: Niural Authentication API
  slug: niural-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-authentication-api-openapi.yml
- filename: niural-contracts-api-openapi.yml
  format: yaml
  label: Niural Contracts API
  slug: niural-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-contracts-api-openapi.yml
- filename: niural-invoices-api-openapi.yml
  format: yaml
  label: Niural Invoices API
  slug: niural-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-invoices-api-openapi.yml
- filename: niural-transactions-api-openapi.yml
  format: yaml
  label: Niural Transactions API
  slug: niural-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-transactions-api-openapi.yml
certifications:
- SOC 2 Type II
description: Niural runs a hosted trust center at trust.niural.com. It returns HTTP 200 but the page is a JavaScript shell — an 814-byte HTML document whose only content is the heading "Trust Center" and a script tag loading laika-app-prod.s3.amazonaws.com/static/trust-center/assets/index.js. Nothing about certifications, subprocessors, or policies is machine-readable, and the automated probe therefore could not confirm a single named certification from the trust center itself. The one certification Niural does publish in readable HTML is a "SOC Type-2" badge in the footer of its marketing site.
kind: trust-center
layout: security
name: Niural Trust Center
name_suffix: Trust Center
overview: Niural maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Niural
provider_slug: niural
slug: niural-trust-center
source_filename: niural-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nprobe: true\nurl: https://trust.niural.com/\ndescription: >-\n  Niural runs a hosted trust center at trust.niural.com. It returns HTTP 200 but\n  the page is a JavaScript shell — an 814-byte HTML document whose only content is\n  the heading \"Trust Center\" and a script tag loading\n  laika-app-prod.s3.amazonaws.com/static/trust-center/assets/index.js. Nothing\n  about certifications, subprocessors, or policies is machine-readable, and the\n  automated probe therefore could not confirm a single named certification from\n  the trust center itself. The one certification Niural does publish in readable\n  HTML is a \"SOC Type-2\" badge in the footer of its marketing site.\nplatform: Laika / Thoropass hosted trust center\ncertifications:\n- name: SOC 2 Type II\n  source: https://www.niural.com/ (footer badge, soc-type-2.svg)\n  report_public: false\nsubprocessors: null\nevidence:\n- {source: 'https://trust.niural.com/', http_status: 200,\
  \ content_type: 'text/html; charset=utf-8', bytes: 814, note: 'JS-rendered shell; no certification text in the served HTML'}\n- {source: 'https://www.niural.com/', http_status: 200, note: 'footer renders a SOC Type-2 badge'}\n- {source: 'https://www.niural.com/pricing', http_status: 200, note: 'same SOC Type-2 footer badge'}\n- {source: 'https://www.niural.com/trust', http_status: 404}\n- {source: 'https://www.niural.com/security', http_status: 404}\ngaps:\n- The trust center serves no server-rendered content, so no crawler, agent, or\n  procurement bot can read Niural's certification list.\n- No subprocessor list, no SOC 2 report request flow, and no compliance page\n  linked from the main site navigation or footer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/security/niural-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Payroll
- Human Resources
- Employer of Record
- Contractor Management
- Global Payments
- Invoicing
- Compliance
- Fintech
trust_url: https://trust.niural.com/
---
