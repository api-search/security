---
api_specs:
- filename: brandcast-account-api-openapi.yml
  format: yaml
  label: Brandcast Account API
  slug: brandcast-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-account-api-openapi.yml
- filename: brandcast-salesforce-api-openapi.yml
  format: yaml
  label: Brandcast Salesforce API
  slug: brandcast-salesforce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-salesforce-api-openapi.yml
- filename: brandcast-templates-api-openapi.yml
  format: yaml
  label: Brandcast Templates API
  slug: brandcast-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-templates-api-openapi.yml
- filename: brandcast-websites-api-openapi.yml
  format: yaml
  label: Brandcast Websites API
  slug: brandcast-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-websites-api-openapi.yml
certifications:
- count
- named
- note
description: ''
kind: trust-center
layout: security
name: Brandcast Trust Center
name_suffix: Trust Center
overview: Brandcast maintains a public trust center documenting count, named, and note compliance.
provider_name: Brandcast
provider_slug: brandcast
slug: brandcast-trust-center
source_filename: brandcast-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://support.timesites.com/en/articles/966545-security-overview\ndocs: https://support.timesites.com/en/articles/966545-security-overview\ntrust_center:\n  published: false\n  url: null\n  note: >-\n    Brandcast / Sites runs no trust centre. There is no trust.<domain> host, no\n    compliance portal and no certification page. What exists is a single\n    prose \"Security Overview\" help-centre article plus an IT FAQ. Recorded here\n    because it is the provider's only published security posture statement.\ncertifications:\n  count: 0\n  named: []\n  note: >-\n    NO certification is claimed anywhere — no SOC 2, no ISO 27001, no PCI DSS,\n    no HIPAA, no FedRAMP, no GDPR attestation. Because no certification or\n    compliance program is published, NO `Compliance` pointer is emitted in\n    apis.yml.\npractices_published:\n- area: hosting\n  claim: Runs on Amazon Web Services across multiple availability zones with firewall\
  \ protection.\n- area: transport-encryption\n  claim: The SITES Studio is served exclusively over SSL; all data is encrypted in transit.\n- area: custom-domain-tls\n  claim: >-\n    Automatic SSL for custom domains for paid customers, using AWS Certificate\n    Manager with automatic annual renewal.\n- area: backups\n  claim: Regular database backups stored across multiple AWS availability zones.\n- area: access-control\n  claim: Employees do not have access to user data unless required for support reasons.\n- area: payments\n  claim: Payments handled by Stripe; card data is never stored on Brandcast servers.\n- area: credential-handling\n  claim: >-\n    Passwords and other sensitive information are filtered from logs; all\n    passwords are one-way hashed with an industry-standard algorithm.\n- area: ddos\n  claim: AWS Shield DDoS protection in front of published websites on CloudFront.\n  source: https://support.timesites.com/en/articles/4774193-sites-web-hosting-platform\n- area: customer-pentest\n\
  \  claim: Customer penetration tests and security scans are permitted when arranged in advance.\n  source: https://support.timesites.com/en/articles/969034-sites-platform-faq-for-it\n- area: accessibility\n  claim: Publishes an ADA-compliance note for websites built on the platform.\n  source: https://support.timesites.com/en/articles/1132211-accessibility-of-sites-websites-ada-compliance\nsubprocessors_published: false\ndata_residency_published: false\nevidence:\n- url: https://support.timesites.com/en/articles/966545-security-overview\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://support.timesites.com/en/articles/969034-sites-platform-faq-for-it\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/security/brandcast-trust-center.yml
summary_line: count, named, note
tags:
- Company
- Enterprise Software
- No-Code
- Website Builder
- Content Management
- Digital Experience
- Web Design
- Brand Management
trust_url: ''
---
