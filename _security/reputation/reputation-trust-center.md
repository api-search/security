---
api_specs:
- filename: reputation-asset-library-api-openapi.yml
  format: yaml
  label: Reputation Asset Library API
  slug: reputation-asset-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-asset-library-api-openapi.yml
- filename: reputation-authorize-api-openapi.yml
  format: yaml
  label: Reputation Authorize API
  slug: reputation-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-authorize-api-openapi.yml
- filename: reputation-categories-api-openapi.yml
  format: yaml
  label: Reputation Categories API
  slug: reputation-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-categories-api-openapi.yml
- filename: reputation-credentials-api-openapi.yml
  format: yaml
  label: Reputation Credentials API
  slug: reputation-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-credentials-api-openapi.yml
- filename: reputation-listing-audits-api-openapi.yml
  format: yaml
  label: Reputation Listing Audits API
  slug: reputation-listing-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-listing-audits-api-openapi.yml
- filename: reputation-locations-api-openapi.yml
  format: yaml
  label: Reputation Locations API
  slug: reputation-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-locations-api-openapi.yml
- filename: reputation-metrics-api-openapi.yml
  format: yaml
  label: Reputation Metrics API
  slug: reputation-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-metrics-api-openapi.yml
- filename: reputation-reports-api-openapi.yml
  format: yaml
  label: Reputation Reports API
  slug: reputation-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reports-api-openapi.yml
- filename: reputation-requests-api-openapi.yml
  format: yaml
  label: Reputation Requests API
  slug: reputation-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-requests-api-openapi.yml
- filename: reputation-reviews-api-openapi.yml
  format: yaml
  label: Reputation Reviews API
  slug: reputation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reviews-api-openapi.yml
- filename: reputation-rich-content-api-openapi.yml
  format: yaml
  label: Reputation Rich Content API
  slug: reputation-rich-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-rich-content-api-openapi.yml
- filename: reputation-summary-api-openapi.yml
  format: yaml
  label: Reputation Summary API
  slug: reputation-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-summary-api-openapi.yml
- filename: reputation-surveys-api-openapi.yml
  format: yaml
  label: Reputation Surveys API
  slug: reputation-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-surveys-api-openapi.yml
- filename: reputation-tenants-api-openapi.yml
  format: yaml
  label: Reputation Tenants API
  slug: reputation-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tenants-api-openapi.yml
- filename: reputation-tickets-api-openapi.yml
  format: yaml
  label: Reputation Tickets API
  slug: reputation-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tickets-api-openapi.yml
- filename: reputation-users-api-openapi.yml
  format: yaml
  label: Reputation Users API
  slug: reputation-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-users-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- HIPAA
- GDPR
- Gramm-Leach-Bliley Act Safeguards Rule
- CCPA
description: ''
kind: trust-center
layout: security
name: Reputation Trust Center
name_suffix: Trust Center
overview: Reputation maintains a public trust center documenting SOC 2 Type II, ISO 27001, HIPAA, GDPR, Gramm-Leach-Bliley Act Safeguards Rule, and CCPA compliance.
provider_name: Reputation
provider_slug: reputation
slug: reputation-trust-center
source_filename: reputation-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://reputation.com/security-posture/\nnote: >-\n  probe-security-programs.py found no trust.reputation.com or security.reputation.com host (both\n  fail to resolve) and no /trust, /security or /compliance path on reputation.com (all 404).\n  Reputation's trust surface is instead a \"Security Posture\" page linked from\n  https://reputation.com/legal-information, fetched 2026-08-13 (HTTP 200), which names its\n  certifications directly. Upgraded from the probe by search.\ncertifications:\n- SOC 2 Type II\n- ISO 27001\n- HIPAA\n- GDPR\n- Gramm-Leach-Bliley Act Safeguards Rule\n- CCPA\npractices:\n  penetration_testing: Conducted by an independent third-party assessor at least annually.\n  encryption_at_rest: AES symmetric block cipher.\n  encryption_in_transit: TLS, with a published approved-cipher policy in the API documentation.\n  password_storage: One-way bcrypt with random salt; 4096+ bit public/private key\
  \ encryption for retrieval.\n  data_residency: Geographically separated US and EU data regions, reflected in separate API hosts.\ndocuments_available_on_request:\n- {name: SOC 2 Type II report, access: under NDA}\n- {name: ISO 27001 certificate, access: under NDA}\nrelated_pages:\n- {name: HIPAA Compliance, url: 'https://reputation.com/hipaa-compliance/'}\n- {name: CCPA Compliance FAQ, url: 'https://reputation.com/ccpa-compliance/'}\n- {name: Data Processing Addendum, url: 'https://reputation.com/reputation-data-processing-addendum/'}\n- {name: Subprocessors, url: 'https://reputation.com/legal-information/reputation-com-subprocessors/'}\nevidence:\n- {source: 'https://reputation.com/security-posture/', http_status: 200, keywords: [soc 2 type ii, iso 27001, hipaa, gdpr, penetration test, encryption]}\n- {source: 'https://reputation.com/hipaa-compliance/', http_status: 200}\n- {source: 'https://reputation.com/legal-information', http_status: 200}\ngaps:\n  vulnerability_disclosure: >-\n\
  \    NONE FOUND. No security.txt (404 on all hosts), no /responsible-disclosure, /security or\n    /vulnerability-disclosure page (all 404), no bug bounty on HackerOne/Bugcrowd/Intigriti, and no\n    security@ contact published on the security-posture page. No Security or VulnerabilityDisclosure\n    pointer is wired in apis.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/security/reputation-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, HIPAA, GDPR, Gramm-Leach-Bliley Act Safeguards Rule, CCPA
tags:
- Reputation Management
- Online Reviews
- Business Listings
- Surveys
- Social Listening
- Competitive Intelligence
- Customer Experience
- Local SEO
trust_url: https://reputation.com/security-posture/
---
