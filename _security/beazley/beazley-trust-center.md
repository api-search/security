---
api_specs:
- filename: beazley-data-capture-quote-and-risk-data-v2.yml
  format: yaml
  label: 'Beazley Data Capture: Quote and Risk Data v2'
  slug: beazley-data-capture-quote-and-risk-data-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-data-capture-quote-and-risk-data-v2.yml
- filename: beazley-data-capture-quote-and-risk-data.yml
  format: yaml
  label: 'Beazley Data Capture: Quote and Risk Data v1'
  slug: beazley-data-capture-quote-and-risk-data-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-data-capture-quote-and-risk-data.yml
- filename: beazley-data-capture-quote-and-risk-data-v3-pre-release.yml
  format: yaml
  label: 'Beazley Data Capture: Quote and Risk Data v3 (pre-release)'
  slug: beazley-data-capture-quote-and-risk-data-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-data-capture-quote-and-risk-data-v3-pre-release.yml
- filename: beazley-compliance-web-api.yml
  format: yaml
  label: Beazley Compliance Web API
  slug: beazley-compliance-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-compliance-web-api.yml
- filename: beazley-broker-and-insured-marketing-data-v2.yml
  format: yaml
  label: Beazley Broker and Insured Marketing Data v2
  slug: beazley-broker-and-insured-marketing-data-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-broker-and-insured-marketing-data-v2.yml
- filename: beazley-currency-exchange.yml
  format: yaml
  label: Beazley Currency Exchange
  slug: beazley-currency-exchange
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-currency-exchange.yml
- filename: beazley-about-beazley.yml
  format: yaml
  label: About Beazley
  slug: beazley-about-beazley
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-about-beazley.yml
- filename: beazley-fast-reader.yml
  format: yaml
  label: Beazley Fast Reader
  slug: beazley-fast-reader
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-fast-reader.yml
- filename: beazley-simple-raters.yml
  format: yaml
  label: Beazley Simple Raters
  slug: beazley-simple-raters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-simple-raters.yml
certifications:
- ISO/IEC 27001
- ISO/IEC 27701
- SOC 2 Type 2
description: Beazley plc publishes no trust centre, no security page and no certification list for itself or for the developer.beazley.com API platform — probes of trust.beazley.com, www.beazley.com/security and www.beazley.com/en-gb/security all miss (the corporate site soft-404s every unknown path with an HTTP 200). The group does operate one real trust centre, at trust.beazley.security, belonging to Beazley Security, the wholly-owned cyber-security services arm created out of the Lodestone business. It publishes gated document access for certifications, policies, service descriptions and a subprocessor list.
kind: trust-center
layout: security
name: Beazley Trust Center
name_suffix: Trust Center
overview: Beazley maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 27701, and SOC 2 Type 2 compliance.
provider_name: Beazley
provider_slug: beazley
slug: beazley-trust-center
source_filename: beazley-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nurl: https://trust.beazley.security/\nentity: Beazley Security\nscope: subsidiary\ndescription: >-\n  Beazley plc publishes no trust centre, no security page and no certification list for itself or for\n  the developer.beazley.com API platform — probes of trust.beazley.com, www.beazley.com/security and\n  www.beazley.com/en-gb/security all miss (the corporate site soft-404s every unknown path with an\n  HTTP 200). The group does operate one real trust centre, at trust.beazley.security, belonging to\n  Beazley Security, the wholly-owned cyber-security services arm created out of the Lodestone\n  business. It publishes gated document access for certifications, policies, service descriptions and\n  a subprocessor list.\ncertifications:\n  - ISO/IEC 27001\n  - ISO/IEC 27701\n  - SOC 2 Type 2\ncertification_note: >-\n  Achieved in 2025 and announced as covering the entire Beazley Security organisation and its\n  globally delivered\
  \ services. They do not certify the Beazley plc API platform.\ndocuments_listed:\n  - Compliance certifications (ISO/IEC 27001, ISO/IEC 27701, SOC 2 Type 2)\n  - Internal Security Controls Policy\n  - Data Processing Agreement\n  - Terms of Service\n  - Service descriptions (Advisory Services, Exposure Management, Incident Response, Third-Party Risk Monitoring)\n  - Subprocessor list\naccess: >-\n  Document downloads are request-gated through the trust centre; the certification and framework list\n  itself is publicly visible.\nevidence:\n  - source: https://trust.beazley.security/\n    status: 200\n    keywords: [SOC 2 Type 2, ISO/IEC 27001, ISO/IEC 27701, penetration test, subprocessors]\n  - source: https://beazley.security/news/beazley-security-simultaneously-achieves-three-cybersecurity-industry-certifications\n    status: 200\n    keywords: [ISO 27001, ISO 27701, SOC 2 Type 2]\nmisses:\n  - {url: 'https://trust.beazley.com', result: DNS does not resolve}\n  - {url: 'https://www.beazley.com/security',\
  \ result: 'HTTP 200 but serves the site 404 page'}\n  - {url: 'https://www.beazley.com/en-gb/security', result: 'HTTP 200 but serves the site 404 page'}\n  - {url: 'https://beazley.security/trust', result: 404}\n  - {url: 'https://beazley.security/certifications', result: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/security/beazley-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 27701, SOC 2 Type 2
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Cyber Insurance
- Specialty Insurance
- Lloyd's of London
- Underwriting
- Risk Data
- Broker
- Carrier
trust_url: https://trust.beazley.security/
---
