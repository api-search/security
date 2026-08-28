---
api_specs:
- filename: algolia-search-api-openapi.yml
  format: yaml
  label: Algolia Search API
  slug: algolia-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-search-api-openapi.yml
- filename: algolia-insights-api-openapi.yml
  format: yaml
  label: Algolia Insights API
  slug: algolia-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-insights-api-openapi.yml
- filename: algolia-recommend-api-openapi.yml
  format: yaml
  label: Algolia Recommend API
  slug: algolia-recommend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-recommend-api-openapi.yml
- filename: algolia-analytics-api-openapi.yml
  format: yaml
  label: Algolia Analytics API
  slug: algolia-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-analytics-api-openapi.yml
- filename: algolia-abtesting-v3-api-openapi.yml
  format: yaml
  label: Algolia A/B Testing API
  slug: algolia-ab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-abtesting-v3-api-openapi.yml
- filename: algolia-personalization-api-openapi.yml
  format: yaml
  label: Algolia Personalization API
  slug: algolia-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-personalization-api-openapi.yml
- filename: algolia-advanced-personalization-api-openapi.yml
  format: yaml
  label: Algolia Advanced Personalization API
  slug: algolia-advanced-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-advanced-personalization-api-openapi.yml
- filename: algolia-crawler-api-openapi.yml
  format: yaml
  label: Algolia Crawler API
  slug: algolia-crawler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-crawler-api-openapi.yml
- filename: algolia-ingestion-api-openapi.yml
  format: yaml
  label: Algolia Ingestion API
  slug: algolia-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-ingestion-api-openapi.yml
- filename: algolia-query-suggestions-api-openapi.yml
  format: yaml
  label: Algolia Query Suggestions API
  slug: algolia-query-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-query-suggestions-api-openapi.yml
- filename: algolia-composition-api-openapi.yml
  format: yaml
  label: Algolia Composition API
  slug: algolia-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-composition-api-openapi.yml
- filename: algolia-agent-studio-api-openapi.yml
  format: yaml
  label: Algolia Agent Studio API
  slug: algolia-agent-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-agent-studio-api-openapi.yml
- filename: algolia-monitoring-api-openapi.yml
  format: yaml
  label: Algolia Monitoring API
  slug: algolia-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-monitoring-api-openapi.yml
certifications:
- read
- named
- reason
- probed
description: Algolia publishes a Vanta-hosted Trust Center at trust.algolia.com. It is the canonical destination for Algolia's compliance posture - the older marketing page at /distributed-secure/security-compliance/ now 301s to it, and www.algolia.com/security serves the same Trust Center application.
kind: trust-center
layout: security
name: Algolia Trust Center
name_suffix: Trust Center
overview: Algolia maintains a public trust center documenting read, named, reason, and probed compliance.
provider_name: Algolia
provider_slug: algolia
slug: algolia-trust-center
source_filename: algolia-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "specification: API Commons Trust Center\nspecificationVersion: '0.1'\nprovider: Algolia\nproviderId: algolia\ngenerated: '2026-08-27'\nmethod: probed\nsource: https://trust.algolia.com\ndescription: >-\n  Algolia publishes a Vanta-hosted Trust Center at trust.algolia.com. It is the canonical destination for Algolia's\n  compliance posture - the older marketing page at /distributed-secure/security-compliance/ now 301s to it, and\n  www.algolia.com/security serves the same Trust Center application.\ntrust_center:\n  url: https://trust.algolia.com\n  http_status: 200\n  title: Algolia Trust Center\n  canonical: https://trust.algolia.com\n  vendor: Vanta\n  vendor_evidence: 'content-location header points at https://assets.vanta.com/static/index-trust-report.<hash>.html'\n  redirects_from:\n    - url: https://www.algolia.com/distributed-secure/security-compliance/\n      status: 301\n      target: https://trust.algolia.com/\n    - url: https://www.algolia.com/security\n      status:\
  \ 200\n      note: Serves the same Vanta Trust Center application.\ncertifications:\n  read: false\n  named: []\n  reason: >-\n    NOT recorded, deliberately. The Vanta Trust Center renders its certification list client-side - the served HTML\n    is a 6.4 KB application shell with the certification data fetched by JavaScript, and the Vanta API endpoint\n    behind it returns 401 Unauthorized to an anonymous caller. The supporting Algolia article\n    (support.algolia.com/hc/en-us/articles/4406981951889 \"What is Algolia's product compliance?\") returns HTTP 403\n    to automated fetches behind a Cloudflare bot challenge. Algolia's own llms.txt asserts \"SOC2, GDPR, HIPAA\n    compliance details\" behind that link, but that is a marketing summary line and not a machine-readable\n    attestation, so no certification name is asserted in this artifact. A human in a browser can read the list;\n    an agent cannot.\n  probed:\n    - url: https://trust.algolia.com\n      status: 200\n      note:\
  \ 'JS-rendered SPA shell; no certification names in the served HTML.'\n    - url: https://api.vanta.com/v1/trust-centers/35qkoispbisbf5si15k7o\n      status: 401\n      note: Unauthorized.\n    - url: https://support.algolia.com/hc/en-us/articles/4406981951889-What-is-Algolia-s-product-compliance-\n      status: 403\n      note: Cloudflare bot challenge.\ncompliance_program:\n  published: true\n  evidence: >-\n    A dedicated, canonical, vendor-operated Trust Center reachable at a first-party subdomain, with a 301 from the\n    provider's own security page. That establishes a published compliance program even though the individual\n    attestations were not machine-readable.\nrelated_security_documentation:\n  - name: Shared responsibility model\n    url: https://www.algolia.com/doc/guides/security/security-best-practices/in-depth/shared-responsibility.md\n    note: >-\n      States Algolia is responsible for \"remaining compliant with standards and certifications\" and for\n      \"letting\
  \ you know about potential vulnerabilities\", and documents SAML SSO and AES256 encryption\n      (Algolia Vault) as Enterprise add-ons.\n  - name: Security best practices\n    url: https://www.algolia.com/doc/guides/security/security-best-practices\n  - name: Algolia Vault\n    url: https://www.algolia.com/doc/guides/security/algolia-vault\n    note: AES256 encryption at rest, Enterprise add-on.\n  - name: API key restrictions\n    url: https://www.algolia.com/doc/guides/security/api-keys/in-depth/api-key-restrictions\npolicies:\n  terms_of_service:\n    url: https://www.algolia.com/policies/terms/\n    status: 200\n  privacy_policy:\n    url: https://www.algolia.com/policies/privacy/\n    status: 200\n  sla:\n    url: https://www.algolia.com/policies/sla/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/security/algolia-trust-center.yml
summary_line: read, named, reason, probed
tags:
- Search
- Discovery
- Recommendations
- Personalization
- Analytics
- E-Commerce
- AI
- Agents
- MCP
- Indexing
trust_url: ''
---
