---
api_specs:
- filename: mailerlite-automations-api-openapi.yml
  format: yaml
  label: MailerLite Automations API
  slug: mailerlite-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-automations-api-openapi.yml
- filename: mailerlite-campaigns-api-openapi.yml
  format: yaml
  label: MailerLite Campaigns API
  slug: mailerlite-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-campaigns-api-openapi.yml
- filename: mailerlite-fields-api-openapi.yml
  format: yaml
  label: MailerLite Fields API
  slug: mailerlite-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-fields-api-openapi.yml
- filename: mailerlite-forms-api-openapi.yml
  format: yaml
  label: MailerLite Forms API
  slug: mailerlite-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-forms-api-openapi.yml
- filename: mailerlite-groups-api-openapi.yml
  format: yaml
  label: MailerLite Groups API
  slug: mailerlite-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-groups-api-openapi.yml
- filename: mailerlite-segments-api-openapi.yml
  format: yaml
  label: MailerLite Segments API
  slug: mailerlite-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-segments-api-openapi.yml
- filename: mailerlite-subscribers-api-openapi.yml
  format: yaml
  label: MailerLite Subscribers API
  slug: mailerlite-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-subscribers-api-openapi.yml
- filename: mailerlite-webhooks-api-openapi.yml
  format: yaml
  label: MailerLite Webhooks API
  slug: mailerlite-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-webhooks-api-openapi.yml
certifications:
- ISO/IEC 27001:2022
- PCI DSS
- GDPR
- EU-U.S. Data Privacy Framework
- Swiss-U.S. Data Privacy Framework
- UK Extension to the EU-U.S. Data Privacy Framework
description: ''
kind: trust-center
layout: security
name: Mailerlite Trust Center
name_suffix: Trust Center
overview: MailerLite maintains a public trust center documenting ISO/IEC 27001:2022, PCI DSS, GDPR, EU-U.S. Data Privacy Framework, Swiss-U.S. Data Privacy Framework, and UK Extension to the EU-U.S. Data Privacy Framework compliance.
provider_name: MailerLite
provider_slug: mailerlite
slug: mailerlite-trust-center
source_filename: mailerlite-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.mailerlite.com/trust-page\nsource: https://www.mailerlite.com/trust-page\nnotes: >-\n  MailerLite publishes a security & compliance page at\n  https://www.mailerlite.com/trust-page (HTTP 200, fetched 2026-08-13), found\n  through the sitemap rather than through any conventional trust-center\n  hostname. It is a narrative page, not a document portal — there is no\n  self-serve audit-report download, no live control status, and no\n  subprocessor list on the page itself.\n\n  IMPORTANT NEGATIVE: trust.mailerlite.com and security.mailerlite.com BOTH\n  return HTTP 200, but they serve the identical 20,689-byte application shell\n  that a deliberately non-existent control hostname also returns. They are a\n  wildcard SPA catch-all, not trust centers, and were rejected as false\n  positives. Only the /trust-page path is real.\n\ncertifications:\n  - ISO/IEC 27001:2022\n  - PCI DSS\n  - GDPR\n  - EU-U.S. Data\
  \ Privacy Framework\n  - Swiss-U.S. Data Privacy Framework\n  - UK Extension to the EU-U.S. Data Privacy Framework\n\ncertification_detail:\n  - {name: \"ISO/IEC 27001:2022\", kind: certification, scope: Information Security Management System (ISMS)}\n  - {name: \"PCI DSS\", kind: compliance, scope: \"Attributed to payment processors in MailerLite's payment path rather than to a MailerLite-held certification — read the page wording before treating this as MailerLite's own attestation.\"}\n  - {name: \"EU-U.S. Data Privacy Framework\", kind: transfer-mechanism}\n  - {name: \"Swiss-U.S. Data Privacy Framework\", kind: transfer-mechanism}\n  - {name: \"UK Extension to EU-U.S. DPF\", kind: transfer-mechanism}\n  - {name: \"GDPR\", kind: regulation, scope: \"Dedicated compliance page at https://www.mailerlite.com/gdpr-compliance (HTTP 200).\"}\n\nnot_published:\n  items:\n    - SOC 2 Type I or Type II\n    - ISO 27017\n    - ISO 27018\n    - ISO 27701\n    - HIPAA\n    - FedRAMP\n    - CSA\
  \ STAR\n  note: >-\n    None of these appears on the trust page. SOC 2 in particular is absent —\n    notable for a platform at MailerLite's scale, and the most likely question a\n    procurement reviewer will ask.\n\nsections:\n  - We have a strong Information Security Policy\n  - We continually develop tools to be GDPR compliant\n  - We're certified to global security and privacy standards\n  - We prioritize infrastructure and network security\n  - We encrypt data communications and minimize retention\n  - We take application and product security seriously\n  - We monitor everything and have a clear plan for response\n  - We have strong corporate and organizational security\n  - We design reliable systems\n\nrelated_documents:\n  privacy_policy: https://www.mailerlite.com/legal/privacy-policy\n  data_processing_addendum: https://www.mailerlite.com/legal/data-processing-agreement\n  gdpr: https://www.mailerlite.com/gdpr-compliance\n  anti_spam_policy: https://www.mailerlite.com/legal/anti-spam-policy\n\
  \  ai_policy: https://www.mailerlite.com/legal/ai-policy\n  responsible_disclosure: https://www.mailerlite.com/legal/responsible-disclosure-program\n  security_incident_notice: https://www.mailerlite.com/newsroom/securityincidentnotice\n\nevidence:\n  - source: https://www.mailerlite.com/trust-page\n    status: 200\n    fetched: '2026-08-13'\n    keywords: [iso/iec 27001:2022, pci-dss, gdpr, data privacy framework, information security policy]\n  - source: https://www.mailerlite.com/legal\n    status: 200\n    fetched: '2026-08-13'\n    keywords: [data processing addendum, privacy policy, responsible disclosure program]\n  - source: https://trust.mailerlite.com/\n    status: 200\n    fetched: '2026-08-13'\n    verdict: rejected\n    reason: \"Wildcard SPA shell — byte-identical in size to a probe of a non-existent subdomain.\"\n  - source: https://security.mailerlite.com/\n    status: 200\n    fetched: '2026-08-13'\n    verdict: rejected\n    reason: \"Wildcard SPA shell — same false positive\
  \ as trust.mailerlite.com.\"\n\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/security/mailerlite-trust-center.yml
summary_line: ISO/IEC 27001:2022, PCI DSS, GDPR, EU-U.S. Data Privacy Framework, Swiss-U.S. Data Privacy Framework, UK Extension to the EU-U.S. Data Privacy Framework
tags:
- Email Marketing
- Automation
- Newsletters
- Subscribers
- Campaigns
- Webhook
- E-Commerce
- Segmentation
- Transactional Email
- MCP
trust_url: https://www.mailerlite.com/trust-page
---
