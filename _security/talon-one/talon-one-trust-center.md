---
api_specs:
- filename: talon-one-integration-api-openapi.yml
  format: yaml
  label: Talon.One Integration API
  slug: talon-one-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-integration-api-openapi.yml
- filename: talon-one-management-api-openapi.yml
  format: yaml
  label: Talon.One Management API
  slug: talon-one-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-management-api-openapi.yml
- filename: talon-one-third-party-api-openapi.yml
  format: yaml
  label: Talon.One Third-party API
  slug: talon-one-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-third-party-api-openapi.yml
- filename: talon-one-shopify-integration-api-openapi.yml
  format: yaml
  label: Talon.One Shopify Integration API
  slug: talon-one-shopify-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-shopify-integration-api-openapi.yml
- filename: talon-one-outbound-notifications-openapi.yml
  format: yaml
  label: Talon.One Outbound Notifications
  slug: talon-one-outbound-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-outbound-notifications-openapi.yml
certifications:
- ISO 27001
- SOC 2
- GDPR
description: Talon.One runs a Vanta-hosted trust center at trust.talon.one and displays certification badges on its marketing site, including a downloadable ISO 27001 certificate.
kind: trust-center
layout: security
name: Talon One Trust Center
name_suffix: Trust Center
overview: Talon.One maintains a public trust center documenting ISO 27001, SOC 2, and GDPR compliance.
provider_name: Talon.One
provider_slug: talon-one
slug: talon-one-trust-center
source_filename: talon-one-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://trust.talon.one\nprovider: Talon.One\nproviderId: talon-one\ndescription: Talon.One runs a Vanta-hosted trust center at trust.talon.one and displays certification\n  badges on its marketing site, including a downloadable ISO 27001 certificate.\nurl: https://trust.talon.one\nplatform: Vanta Trust Center\nhttp_status: 200\nmachine_readable: false\nrendering_note: 'The trust center is a client-side rendered Vanta trust report: the HTML shell is 7 KB\n  and carries no certification names, so the certifications below were confirmed from Talon.One own marketing\n  site and the certificate PDF it links, not scraped from the trust page.'\ncertifications:\n- name: ISO 27001\n  status: certified\n  evidence: https://9425930.fs1.hubspotusercontent-na1.net/hubfs/9425930/Other/ISO%20certification%20Talon.One.pdf\n  evidence_status: 200\n- name: SOC 2\n  status: claimed\n  evidence: Badge and site copy on https://www.talon.one/ — \"\
  compliant with SOC 2, ISO, and GDPR\"; the\n    report itself is behind the trust center request flow.\n- name: GDPR\n  status: claimed\n  evidence: Badge on https://www.talon.one/ and https://www.talon.one/legal/privacy-policy.\ndocuments:\n- name: Vanta document library\n  url: https://app.vanta.com/doc?s=c0ytzpybh1189xxgiu1dkd\n  note: Linked from the trust center; access is request-gated.\nsecurity_features:\n- name: Two-factor authentication\n  docs: https://docs.talon.one/docs/product/account/account-settings/set-up-2fa\n- name: Roles and permissions\n  docs: https://docs.talon.one/docs/product/account/account-settings/manage-roles\n- name: Audit logs\n  docs: https://docs.talon.one/docs/product/account/logs/audit-logs\n- name: Scoped API keys\n  note: Management API keys are created by an admin with an explicit endpoint allow-list and a mandatory\n    expiration date.\n- name: Customer data deletion\n  note: Integration API deleteCustomerData removes a customer profile and its data\
  \ by integration id.\nvulnerability_disclosure:\n  published: false\n  note: No security.txt on any host and no bug bounty or coordinated disclosure page found on talon.one;\n    probe-security-programs.py returned vdp=none.\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/security/talon-one-trust-center.yml
summary_line: ISO 27001, SOC 2, GDPR
tags:
- Promotions
- Loyalty
- Coupons
- Incentives
- Campaigns
- Personalization
- MarTech
- Rules Engine
- Referrals
- Discounts
- Ecommerce
- Retail
trust_url: https://trust.talon.one
---
