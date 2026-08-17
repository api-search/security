---
api_specs:
- filename: postman.yaml
  format: yaml
  label: LeadSquared REST API
  slug: rest-api
  spec_type: Postman
  url: https://apidocs.leadsquared.com/leadsquared-run-in-postman/
- filename: leadsquared-activities-api-openapi.yml
  format: yaml
  label: LeadSquared Activities API
  slug: leadsquared-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/openapi/leadsquared-activities-api-openapi.yml
- filename: leadsquared-leads-api-openapi.yml
  format: yaml
  label: LeadSquared Leads API
  slug: leadsquared-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/openapi/leadsquared-leads-api-openapi.yml
certifications:
- ISO 27001:2022
- GDPR
description: ''
kind: trust-center
layout: security
name: Leadsquared Trust Center
name_suffix: Trust Center
overview: LeadSquared maintains a public trust center documenting ISO 27001:2022 and GDPR compliance.
provider_name: LeadSquared
provider_slug: leadsquared
slug: leadsquared-trust-center
source_filename: leadsquared-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.leadsquared.com/security/\ntitle: LeadSquared Security\ndedicated_trust_center: false\nnote: >-\n  trust.leadsquared.com does not resolve (curl exit 6, no DNS). LeadSquared's\n  compliance posture is published as a single marketing-site security page rather\n  than a trust portal, and there is no downloadable evidence pack, no subprocessor\n  list and no live control status. The certifications below are as stated on that\n  page; API Evangelist has not seen the certificates themselves.\ncertifications:\n  - name: ISO 27001:2022\n    scope: >-\n      \"applicable across the entire LeadSquared product, cloud services, IT\n      infrastructure, administration, finance, and internal functions\"\n    certifier: British Standards Institute (BSI)\n    self_reported: true\n  - name: GDPR\n    scope: >-\n      Full compliance claimed, including a Data Processing Agreement with Standard\n      Contractual Clauses\
  \ for EU data transfers.\n    self_reported: true\ninherited_certifications:\n  note: >-\n    Stated as properties of the AWS data centres LeadSquared runs on, NOT of\n    LeadSquared itself: \"Our data centers are hosted in AWS are ISO 27001, SSAE-16\n    and HIPAA compliant.\" Recorded separately because infrastructure compliance is\n    not the same claim as product compliance.\n  items: [ISO 27001, SSAE-16, HIPAA]\nnot_claimed: [SOC 2, PCI DSS, FedRAMP, CSA STAR, ISO 27017, ISO 27018]\nnot_claimed_note: >-\n  No SOC 2 or PCI DSS claim appears anywhere on the page — notable for a CRM sold\n  into banking, lending, healthcare and education.\nsector_pages:\n  - {name: Healthcare security and compliance, url: 'https://www.leadsquared.com/healthcare/healthcare-security-and-compliance/'}\nlegal:\n  terms_of_service: https://www.leadsquared.com/leadsquared-terms-of-service/\n  privacy_policy: https://www.leadsquared.com/privacy-policy/\nevidence:\n  - source: https://www.leadsquared.com/security/\n\
  \    http_status: 200\n    fetched: '2026-08-13'\n    keywords: [ISO 27001:2022, British Standards Institute, BSI, GDPR, HIPAA, SSAE-16]\n  - source: https://trust.leadsquared.com/\n    http_status: 0\n    fetched: '2026-08-13'\n    note: DNS/connection failure — no trust subdomain exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/security/leadsquared-trust-center.yml
summary_line: ISO 27001:2022, GDPR
tags:
- Marketing Automation
- CRM
- Sales Automation
- Lead Management
- Customer Engagement
- Field Force Automation
trust_url: https://www.leadsquared.com/security/
---
