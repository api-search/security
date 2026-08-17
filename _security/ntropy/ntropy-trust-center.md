---
api_specs:
- filename: ntropy-account-holder-api-openapi.yml
  format: yaml
  label: Ntropy Account Holder API
  slug: ntropy-account-holder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-account-holder-api-openapi.yml
- filename: ntropy-accountholders-api-openapi.yml
  format: yaml
  label: Ntropy accountHolders API
  slug: ntropy-accountholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-accountholders-api-openapi.yml
- filename: ntropy-bank-statements-api-openapi.yml
  format: yaml
  label: Ntropy Bank statements API
  slug: ntropy-bank-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-bank-statements-api-openapi.yml
- filename: ntropy-bankstatements-api-openapi.yml
  format: yaml
  label: Ntropy bankStatements API
  slug: ntropy-bankstatements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-bankstatements-api-openapi.yml
- filename: ntropy-batches-api-openapi.yml
  format: yaml
  label: Ntropy batches API
  slug: ntropy-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-batches-api-openapi.yml
- filename: ntropy-categories-api-openapi.yml
  format: yaml
  label: Ntropy categories API
  slug: ntropy-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-categories-api-openapi.yml
- filename: ntropy-enrichment-api-openapi.yml
  format: yaml
  label: Ntropy Enrichment API
  slug: ntropy-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-enrichment-api-openapi.yml
- filename: ntropy-entities-api-openapi.yml
  format: yaml
  label: Ntropy entities API
  slug: ntropy-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-entities-api-openapi.yml
- filename: ntropy-labels-api-openapi.yml
  format: yaml
  label: Ntropy Labels API
  slug: ntropy-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-labels-api-openapi.yml
- filename: ntropy-misc-api-openapi.yml
  format: yaml
  label: Ntropy Misc API
  slug: ntropy-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-misc-api-openapi.yml
- filename: ntropy-personalization-api-openapi.yml
  format: yaml
  label: Ntropy personalization API
  slug: ntropy-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-personalization-api-openapi.yml
- filename: ntropy-recurrence-api-openapi.yml
  format: yaml
  label: Ntropy recurrence API
  slug: ntropy-recurrence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-recurrence-api-openapi.yml
- filename: ntropy-reporting-api-openapi.yml
  format: yaml
  label: Ntropy Reporting API
  slug: ntropy-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-reporting-api-openapi.yml
- filename: ntropy-reports-api-openapi.yml
  format: yaml
  label: Ntropy reports API
  slug: ntropy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-reports-api-openapi.yml
- filename: ntropy-transactions-api-openapi.yml
  format: yaml
  label: Ntropy transactions API
  slug: ntropy-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-transactions-api-openapi.yml
- filename: ntropy-webhooks-api-openapi.yml
  format: yaml
  label: Ntropy webhooks API
  slug: ntropy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-webhooks-api-openapi.yml
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Ntropy Trust Center
name_suffix: Trust Center
overview: Ntropy maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Ntropy
provider_slug: ntropy
slug: ntropy-trust-center
source_filename: ntropy-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://trust.ntropy.com/\nplatform: Vanta Trust Center\ntitle: Ntropy Network Trust Center\ncertifications:\n  - SOC 2 Type 2\ncompliance_claims:\n  - id: soc2-type-2\n    claim: \"We are SOC2 Type 2 certified.\"\n    source: https://ntropy.com/\n    location: site footer (with SOC 2 certification badge, linking to the AICPA Trust Services Criteria)\n  - id: gdpr\n    claim: >-\n      Privacy policy names Ntropy Network Inc as the GDPR Data Controller and its\n      service providers as Data Processors; CCPA/CPRA disclosures are also present.\n    source: https://ntropy.com/privacy\nevidence:\n  - source: https://trust.ntropy.com/\n    http_status: 200\n    signals:\n      - \"<title>Ntropy Network Trust Center</title>\"\n      - 'og:title \"Ntropy Network Trust Center\"'\n      - 'canonical https://trust.ntropy.com'\n      - Vanta-hosted trust center (assets.vanta.com / app.vanta.com document links)\n  - source:\
  \ https://ntropy.com/\n    http_status: 200\n    signals:\n      - \"SOC2 SOC certification logo (footer image)\"\n      - \"We are SOC2 Type 2 certified.\"\n  - source: https://ntropy.com/privacy\n    http_status: 200\n    signals: [GDPR, CCPA]\nlimitations: >-\n  The trust center is a client-rendered Vanta single-page app: every path under\n  trust.ntropy.com (including /robots.txt, /sitemap.xml and /.well-known/security.txt)\n  returns the same HTML shell with HTTP 200, and the Vanta public API\n  (api.vanta.com/v1/.../diyk4qgm52zm0ge4dwxm33) answers 401 anonymously. The\n  certification list beyond SOC 2 Type 2, and any downloadable report inventory,\n  therefore require requesting access through the trust center itself and could not\n  be read machine-side. Only the SOC 2 Type 2 claim is recorded because it is\n  independently published, in plain text, on ntropy.com.\nchecked: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/security/ntropy-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- Fintech
- Transaction Enrichment
- Financial Data
- Data Enrichment
- Bank Statements
- Categorization
- Underwriting
trust_url: https://trust.ntropy.com/
---
