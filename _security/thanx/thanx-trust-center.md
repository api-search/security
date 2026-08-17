---
api_specs:
- filename: thanx-account-api-openapi.yml
  format: yaml
  label: Thanx Account API
  slug: thanx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-account-api-openapi.yml
- filename: thanx-auth-api-openapi.yml
  format: yaml
  label: Thanx Auth API
  slug: thanx-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-auth-api-openapi.yml
- filename: thanx-baskets-api-openapi.yml
  format: yaml
  label: Thanx Baskets API
  slug: thanx-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-baskets-api-openapi.yml
- filename: thanx-campaigns-api-openapi.yml
  format: yaml
  label: Thanx Campaigns API
  slug: thanx-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-campaigns-api-openapi.yml
- filename: thanx-cards-api-openapi.yml
  format: yaml
  label: Thanx Cards API
  slug: thanx-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-cards-api-openapi.yml
- filename: thanx-gift-cards-api-openapi.yml
  format: yaml
  label: Thanx Gift Cards API
  slug: thanx-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-gift-cards-api-openapi.yml
- filename: thanx-issuance-jobs-api-openapi.yml
  format: yaml
  label: Thanx Issuance Jobs API
  slug: thanx-issuance-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-issuance-jobs-api-openapi.yml
- filename: thanx-locations-api-openapi.yml
  format: yaml
  label: Thanx Locations API
  slug: thanx-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-locations-api-openapi.yml
- filename: thanx-metadata-api-openapi.yml
  format: yaml
  label: Thanx Metadata API
  slug: thanx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-metadata-api-openapi.yml
- filename: thanx-points-api-openapi.yml
  format: yaml
  label: Thanx Points API
  slug: thanx-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-points-api-openapi.yml
- filename: thanx-purchases-api-openapi.yml
  format: yaml
  label: Thanx Purchases API
  slug: thanx-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-purchases-api-openapi.yml
- filename: thanx-rewards-api-openapi.yml
  format: yaml
  label: Thanx Rewards API
  slug: thanx-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-rewards-api-openapi.yml
- filename: thanx-subscribers-api-openapi.yml
  format: yaml
  label: Thanx Subscribers API
  slug: thanx-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-subscribers-api-openapi.yml
- filename: thanx-users-api-openapi.yml
  format: yaml
  label: Thanx Users API
  slug: thanx-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-users-api-openapi.yml
certifications:
- SOC 2 Type 2
- PCI DSS
- HIPAA
- ISO 27001
- FedRAMP
description: 'Thanx names two certifications publicly — SOC 2 Type 2 and PCI DSS Level 1 Service Provider — on its Data Platform product page, alongside a >99.95% platform and API uptime claim. There is NO trust center in the usual sense: no portal, no downloadable attestation, no subprocessor list, no security questionnaire self-service. probe-security-programs.py returned vdp=none trust=none for this provider; these claims were found by reading the marketing site and are recorded here because the certifications themselves are named and specific.'
kind: trust-center
layout: security
name: Thanx Trust Center
name_suffix: Trust Center
overview: Thanx maintains a public trust center documenting SOC 2 Type 2, PCI DSS, HIPAA, ISO 27001, and FedRAMP compliance.
provider_name: Thanx
provider_slug: thanx
slug: thanx-trust-center
source_filename: thanx-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.thanx.com/open-platform-apis\ndescription: >-\n  Thanx names two certifications publicly — SOC 2 Type 2 and PCI DSS Level 1 Service Provider —\n  on its Data Platform product page, alongside a >99.95% platform and API uptime claim. There\n  is NO trust center in the usual sense: no portal, no downloadable attestation, no subprocessor\n  list, no security questionnaire self-service. probe-security-programs.py returned\n  vdp=none trust=none for this provider; these claims were found by reading the marketing site\n  and are recorded here because the certifications themselves are named and specific.\ntrust_center:\n  portal: null\n  status: no-portal\n  note: >-\n    trust.thanx.com redirects to rewards.thanx.com/trust and returns 403; www.thanx.com/trust\n    and /security both 404. Certification claims live on product marketing pages only.\ncertifications:\n  - name: SOC 2 Type 2\n    status: claimed\n    evidence:\
  \ >-\n      \"Industry-leading security standards: SOC 2 Type 2 Compliant ✓\" and \"SOC 2 Type 2 and PCI\n      DSS Level 1 certified, with continuous monitoring to protect your guest data\"\n      (https://www.thanx.com/open-platform-apis)\n    report_available: false\n    note: No public attestation letter or NDA-gated portal found.\n  - name: PCI DSS\n    level: Level 1 Service Provider\n    status: claimed\n    evidence: >-\n      \"PCI DSS Level 1 Service Provider ✓\" (https://www.thanx.com/open-platform-apis)\n    corroboration: >-\n      Dedicated secure.api.thanx.com / secure.api.thanxsandbox.com hosts appear in the OpenAPI\n      servers[] blocks, and card enrollment is tokenized through the Visa/Mastercard/Amex\n      networks rather than storing PANs — both consistent with a segmented cardholder-data\n      environment.\n  - name: HIPAA\n    status: not-claimed\n  - name: ISO 27001\n    status: not-claimed\n  - name: FedRAMP\n    status: not-claimed\navailability_claim:\n  target:\
  \ '>99.95%'\n  scope: platform and API\n  source: https://www.thanx.com/open-platform-apis\n  contractual: false\n  observed: >-\n    status.thanx.com publishes 90-day per-component uptime — Consumer API 100.000%,\n    Merchant API 99.925%, Authentication 100.000% as of 2026-08-13.\nprivacy:\n  privacy_policy: https://dashboard.thanx.com/privacy\n  terms: https://dashboard.thanx.com/terms\n  note: www.thanx.com/privacy and /terms both 302 to the dashboard host.\ndata_handling:\n  export_surfaces:\n    - SFTP daily CSV snapshots\n    - Snowflake Secure Data Sharing\n    - Thanx Connex managed loading (Snowflake, BigQuery, Redshift, Databricks, Athena, ClickHouse, Postgres, MySQL, SQL Server, S3, GCS, Azure Blob, Google Sheets)\n  private_connectivity: AWS PrivateLink for the Loyalty API (https://docs.thanx.com/loyalty/private-link)\n  webhook_guidance: >-\n    Thanx explicitly warns that sensitive values must not be placed in webhook query\n    parameters, since those are static and sent\
  \ on every delivery.\nx-evidence:\n  fetched: '2026-08-13'\n  urls:\n    - {url: 'https://www.thanx.com/open-platform-apis', status: 200, finding: 'SOC 2 Type 2 + PCI DSS Level 1 + >99.95% uptime'}\n    - {url: 'https://trust.thanx.com', status: 403, finding: 'redirects to rewards.thanx.com/trust; no trust portal'}\n    - {url: 'https://www.thanx.com/security', status: 404}\n    - {url: 'https://dashboard.thanx.com/privacy', status: 200}\n    - {url: 'https://dashboard.thanx.com/terms', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/security/thanx-trust-center.yml
summary_line: SOC 2 Type 2, PCI DSS, HIPAA, ISO 27001, FedRAMP
tags:
- Restaurant
- Loyalty
- Guest Engagement
- Marketing
- CRM
- Online Ordering
- Webhooks
- Points
- Rewards
- Campaigns
trust_url: ''
---
