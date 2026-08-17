---
api_specs:
- filename: mailosaur-analysis-api-openapi.yml
  format: yaml
  label: Mailosaur Analysis API
  slug: mailosaur-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-analysis-api-openapi.yml
- filename: mailosaur-devices-api-openapi.yml
  format: yaml
  label: Mailosaur Devices API
  slug: mailosaur-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-devices-api-openapi.yml
- filename: mailosaur-files-api-openapi.yml
  format: yaml
  label: Mailosaur Files API
  slug: mailosaur-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-files-api-openapi.yml
- filename: mailosaur-messages-api-openapi.yml
  format: yaml
  label: Mailosaur Messages API
  slug: mailosaur-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-messages-api-openapi.yml
- filename: mailosaur-previews-api-openapi.yml
  format: yaml
  label: Mailosaur Previews API
  slug: mailosaur-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-previews-api-openapi.yml
- filename: mailosaur-servers-api-openapi.yml
  format: yaml
  label: Mailosaur Servers API
  slug: mailosaur-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-servers-api-openapi.yml
- filename: mailosaur-usage-api-openapi.yml
  format: yaml
  label: Mailosaur Usage API
  slug: mailosaur-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-usage-api-openapi.yml
certifications:
- ISO 27001:2022
- PCI DSS
- GDPR
- UK Data Protection Act
- CCPA
description: ''
kind: trust-center
layout: security
name: Mailosaur Trust Center
name_suffix: Trust Center
overview: Mailosaur maintains a public trust center documenting ISO 27001:2022, PCI DSS, GDPR, UK Data Protection Act, and CCPA compliance.
provider_name: Mailosaur
provider_slug: mailosaur
slug: mailosaur-trust-center
source_filename: mailosaur-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://trust.mailosaur.com and https://mailosaur.com/security\nurl: https://trust.mailosaur.com\nsecondary_url: https://mailosaur.com/security\nplatform: Vanta (EU tenant — app.eu.vanta.com)\ncertifications:\n- ISO 27001:2022\n- PCI DSS\n- GDPR\n- UK Data Protection Act\n- CCPA\nposture:\n  hosting: Google Cloud Platform, data centres in the EU and the United Kingdom\n  encryption_at_rest: AES-256\n  audits: Regularly audited by independent third-party assessors\n  questionnaires: >-\n    Responds to Vendor Security Alliance (VSA) assessments and provides a\n    Security Assessment Pack on request.\nevidence:\n- source: https://trust.mailosaur.com\n  http_status: 200\n  fetched: '2026-08-14'\n  keywords:\n  - trust center\n  - vanta\n  note: >-\n    A real hosted trust centre, not a marketing page — served from\n    trust.mailosaur.com on Vanta's EU tenant, with the document portal at\n    app.eu.vanta.com. Found\
  \ by subdomain probe; the earlier pass had recorded\n    only the marketing /security page.\n- source: https://mailosaur.com/security\n  http_status: 200\n  fetched: '2026-08-14'\n  keywords:\n  - iso 27001\n  - pci dss\n  - gdpr\n  - ccpa\nnot_found:\n- claim: SOC 2\n  note: Not asserted on either surface.\n- claim: HIPAA\n  note: Not asserted on either surface.\n- claim: FedRAMP\n  note: Not asserted on either surface.\nvulnerability_disclosure:\n  found: false\n  note: >-\n    PROBED 2026-08-14 and not found — no /.well-known/security.txt (404), no\n    /security.txt (404), no /responsible-disclosure,\n    /security/responsible-disclosure or /vulnerability-disclosure page (all 404),\n    no hackerone.com/mailosaur or bugcrowd.com/mailosaur programme (both 404),\n    and no security@ address on the security, contact or privacy pages (which\n    publish sales@, support@ and dpo@ only). No VulnerabilityDisclosure or\n    Security pointer is emitted, because Mailosaur publishes no route\
  \ for\n    reporting a vulnerability.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/security/mailosaur-trust-center.yml
summary_line: ISO 27001:2022, PCI DSS, GDPR, UK Data Protection Act, CCPA
tags:
- Email Testing
- SMS Testing
- Developer Tools
- QA Automation
- CI/CD
- SMTP
- TOTP
- Deliverability
trust_url: https://trust.mailosaur.com
---
