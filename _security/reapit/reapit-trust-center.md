---
certifications:
- ISO 27001
description: Reapit publishes its security posture on a product page under Platform > Infrastructure > Security rather than in a dedicated trust center. The substantive, verifiable claim is ISO 27001 certification with independent third-party audits, backed by an Information Security Management System framework. Single sign-on across the platform and partner integrations, and multi-factor authentication, are named controls. There is no downloadable evidence portal, no SOC 2 report, no sub-processor list, no status-of-controls page and no security questionnaire self-service — so buyers must ask for evidence through sales or the partner team.
kind: trust-center
layout: security
name: Reapit Trust Center
name_suffix: Trust Center
overview: Reapit maintains a public trust center documenting ISO 27001 compliance.
provider_name: Reapit
provider_slug: reapit
slug: reapit-trust-center
source_filename: reapit-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nprobe: false\nprobe_note: >-\n  0-working/probe-security-programs.py returned \"trust=none\" — there is no\n  trust.reapit.com, no /trust and no /compliance path. The security posture is\n  published on a marketing product page instead, which the keyword-threshold\n  probe does not treat as a trust center. Recorded here from a direct read of\n  that page.\nurl: https://www.reapit.com/security\nstatus: 200\ntitle: Security — Keep yours and your clients data safe\ndescription: >-\n  Reapit publishes its security posture on a product page under Platform >\n  Infrastructure > Security rather than in a dedicated trust center. The\n  substantive, verifiable claim is ISO 27001 certification with independent\n  third-party audits, backed by an Information Security Management System\n  framework. Single sign-on across the platform and partner integrations, and\n  multi-factor authentication, are named controls. There is no downloadable\n  evidence\
  \ portal, no SOC 2 report, no sub-processor list, no status-of-controls\n  page and no security questionnaire self-service — so buyers must ask for\n  evidence through sales or the partner team.\ncertifications:\n- name: ISO 27001\n  status: certified\n  scope_note: >-\n    \"Externally audited ISO 27001 accreditation\" covering Reapit's Information\n    Management Security System framework of practices, policies and controls.\n  evidence_url: https://www.reapit.com/security\n  independently_audited: true\ncontrols_published:\n- name: Information Security Management System (ISMS)\n  detail: framework bringing together practices, policies and controls\n- name: Single sign-on\n  detail: one secure login across the Reapit platform and partner integrations\n- name: Multi-factor authentication\n  detail: named as a platform control\n- name: User and client authentication / access permissions\n  detail: >-\n    Per-customer app install grants scoped permissions; uninstall revokes access\n  \
  \  (see scopes/reapit-scopes.yml)\n- name: Webhook payload signing\n  detail: Ed25519 asymmetric signing with per-app key pairs\n- name: Published webhook egress IPs\n  detail: three static eu-west-2 Elastic IPs for firewall allowlisting\n- name: App listing review\n  detail: >-\n    Every AppMarket application passes a Reapit listing review before it can\n    reach any customer's production data\nnot_published:\n- SOC 2 Type I or Type II report\n- PCI DSS attestation\n- HIPAA / FedRAMP (not applicable to this market)\n- CSA STAR listing\n- sub-processor list\n- public penetration-test summary\n- security questionnaire self-service / evidence portal\n- RFC 9116 security.txt\nrelated_pages:\n  privacy_policy: https://www.reapit.com/legal/privacy-policy\n  cookie_policy: https://www.reapit.com/legal/cookie-policy\n  modern_slavery: https://www.reapit.com/legal/modern-slavery-policy\n  terms: https://www.reapit.com/legal/terms-and-conditions\n  developer_terms: https://foundations-documentation.reapit.cloud/developer-terms-and-conditions\n\
  \  partner_bsc: https://www.reapit.com/legal/terms-and-conditions/reapit-partner-business-service-catalogue\n  status: https://status.reapit.com/\nevidence:\n- source: https://www.reapit.com/security\n  keywords: [iso 27001, independent third-party audits, information management security\n      system, single sign on, multi factor authentication]\n  fetched: '2026-07-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reapit/refs/heads/main/security/reapit-trust-center.yml
summary_line: ISO 27001
tags:
- Real Estate
- United Kingdom
- PropTech
- CRM
- Estate Agents
- Property Listings
- Property Management
- Rentals
- Conveyancing
- Australia
trust_url: https://www.reapit.com/security
---
