---
api_specs:
- filename: google-analytics-4-data-v1beta-openapi.yml
  format: yaml
  label: Google Analytics Data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-data-v1beta-openapi.yml
- filename: google-analytics-4-admin-v1beta-openapi.yml
  format: yaml
  label: Google Analytics Admin API
  slug: google-analytics-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-admin-v1beta-openapi.yml
certifications:
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Google Analytics 4 Trust Center
name_suffix: Trust Center
overview: Google Analytics 4 maintains a public trust center documenting ISO 27001 compliance.
provider_name: Google Analytics 4
provider_slug: google-analytics-4
slug: google-analytics-4-trust-center
source_filename: google-analytics-4-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://support.google.com/analytics/answer/6004245\nnote: >-\n  Google runs no trust portal scoped to Google Analytics. trust.google.com,\n  security.analytics.google.com and the usual /trust and /compliance paths do not resolve to\n  a GA4-specific trust center. What Google does publish is a Google-Analytics-specific data\n  privacy and security article that names one certification explicitly and enumerates the\n  data-processing regimes GA4 operates under. Only claims Google makes about Google Analytics\n  by name are recorded here — Google Cloud's much larger certification catalogue is a\n  different product and is deliberately NOT credited to GA4.\nurl: https://support.google.com/analytics/answer/6004245\ncertifications:\n  - name: ISO 27001\n    scope: >-\n      \"Google has earned ISO 27001 certification for the systems, applications, people,\n      technology, processes, and data centers serving a number\
  \ of Google products, including\n      Google Analytics.\"\n    named_for_ga4: true\n    source: https://support.google.com/analytics/answer/6004245\ncompliance_programs:\n  - name: GDPR\n    role: data processor\n    instrument: Google Ads Data Processing Terms\n    source: https://support.google.com/analytics/answer/3379636\n  - name: LGPD (Brazil)\n    role: data processor\n    instrument: Google Ads Data Processing Terms\n  - name: U.S. State Privacy Laws\n    role: service provider / processor\n    instrument: U.S. State Privacy Laws Service Provider and Processor Addendum\n  - name: Google EU User Consent Policy\n    role: publisher obligation\n    applies_to: Google Analytics Advertising Features\nnot_claimed_for_ga4:\n  certifications:\n    - SOC 1\n    - SOC 2\n    - SOC 3\n    - PCI DSS\n    - HIPAA\n    - FedRAMP\n  note: >-\n    None of these are asserted for Google Analytics on any Google page located during this\n    pass. Google Cloud Platform holds all of them, but GCP\
  \ is a separate product with a\n    separate certification scope and crediting them here would misattribute another product's\n    posture.\ndata_handling:\n  privacy_policy: https://policies.google.com/privacy\n  data_processing_terms: https://support.google.com/analytics/answer/3379636\n  cookies: https://policies.google.com/technologies/cookies\n  data_retention_api:\n    resource: DataRetentionSettings\n    operations:\n      - properties_dataRetentionSettings_get\n      - properties_dataRetentionSettings_patch\n    spec: openapi/google-analytics-4-admin-v1beta-openapi.yml\n    note: >-\n      Data retention is programmatically readable and writable, including the userDataRetention\n      field added 2025-01-20. Notable for compliance automation.\n  data_redaction_api:\n    resource: DataRedactionSettings\n    channel: v1alpha\n    note: Per-data-stream redaction of email addresses and URL query parameters.\n  user_deletion_quota:\n    limit: 500\n    scope: per property per day\n\
  \    source: https://developers.google.com/analytics/devguides/config/admin/v1/quotas\nevidence:\n  - source: https://support.google.com/analytics/answer/6004245\n    http_status: 200\n    keywords: [iso 27001, gdpr, lgpd, data processing terms, data processor]\n  - source: https://support.google.com/analytics/answer/3407084\n    http_status: 200\n    kind: Google Analytics data privacy and security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/security/google-analytics-4-trust-center.yml
summary_line: ISO 27001
tags:
- Analytics
- Data Collection
- Marketing
- Measurements
- Mobile Analytics
- Reporting
- Web Analytics
- Attribution
- Audiences
- Event Tracking
trust_url: https://support.google.com/analytics/answer/6004245
---
