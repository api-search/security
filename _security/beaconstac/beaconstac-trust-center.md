---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Uniqode QR Code API
  slug: uniqode-qr-code-api
  spec_type: Postman
  url: https://apidocs.uniqode.com/
certifications:
- SOC 2 Type I
- SOC 2 Type II
- ISO 27001:2022
- HIPAA
- GDPR
- UK GDPR
description: ''
kind: trust-center
layout: security
name: Beaconstac Trust Center
name_suffix: Trust Center
overview: Beaconstac maintains a public trust center documenting SOC 2 Type I, SOC 2 Type II, ISO 27001:2022, HIPAA, GDPR, and UK GDPR compliance.
provider_name: Beaconstac
provider_slug: beaconstac
slug: beaconstac-trust-center
source_filename: beaconstac-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.uniqode.com/\nurl: https://trust.uniqode.com/\n# CURATION NOTE — do not let the keyword probe overwrite this file again.\n# 0-working/probe-security-programs.py keyword-scrapes trust.uniqode.com and returns\n# SOC 2 / ISO 27001 / ISO 27017 / ISO 27018 / HIPAA / FedRAMP / GDPR. Three of those are wrong:\n# ISO 27017, ISO 27018 and FedRAMP appear on the page inside the SUBPROCESSOR records\n# (Datadog carries iso-27017/iso-27018/fedramp-li-saas; Auth0 carries iso-27018/pci), not in\n# Uniqode's own certification set. The trust portal's own vendor record for\n# website https://www.uniqode.com lists exactly:\n#   [\"hipaa\",\"soc2-type-1\",\"soc2-type-2\",\"gdpr\",\"iso-27001-2022\"]\n# which is the list below. This was already corrected in the 2026-07-18 round; the 2026-08-13\n# probe re-introduced the over-claim and it has been reverted a second time.\ncertifications:\n- SOC 2 Type I\n- SOC 2 Type II\n\
  - ISO 27001:2022\n- HIPAA\n- GDPR\n- UK GDPR\nattestations:\n- Penetration test report (updated, per the 2026-02-02 trust-portal announcement)\n- Cyber Security Audit Certification\n- Security policies and controls\nlast_renewal:\n  date: '2026-02-02'\n  announcement: 'Your Data, Our Priority: New Security Updates from Uniqode'\n  renewed: [ISO 27001:2022, SOC 2 Type II, HIPAA, GDPR & UK GDPR]\n  note: Trust portal also enabled a \"Trust Agent\" chat surface for security-questionnaire upload.\nsubprocessors:\n- name: Auth0\n  purpose: Authentication and identity management\n  regions: [US, UK]\n  note: Also backs the auth.uniqode.com OAuth/OIDC authorization server.\n- name: AWS\n  purpose: Data storage\n  regions: [US]\n- name: Datadog\n  purpose: Monitoring and analytics\n  regions: [US]\n- name: Intercom\n  purpose: Customer service communications\n  regions: [US]\n  note: Also hosts docs.uniqode.com, which is why an Intercom security.txt is served there.\n- name: Stripe\n  purpose:\
  \ Payment processing and subscriptions\n  regions: [US]\nevidence:\n- source: https://trust.uniqode.com/\n  http_status: 200\n  keywords: [soc 2 type 1, soc 2 type 2, iso 27001:2022, hipaa, gdpr, trust center]\n- source: https://www.uniqode.com/security\n  http_status: 200\n  keywords: [soc 2 type ii, gdpr, hipaa, iso, sso, saml, 2fa, scanguard]\n- source: https://www.uniqode.com/llms.txt\n  http_status: 200\n  keywords: [soc 2 type ii, iso 27001:2022, hipaa, gdpr]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconstac/refs/heads/main/security/beaconstac-trust-center.yml
summary_line: SOC 2 Type I, SOC 2 Type II, ISO 27001:2022, HIPAA, GDPR, UK GDPR
tags:
- Company
- Big Data
- QR Codes
- Digital Business Cards
- Marketing
- Analytics
- SaaS
- Proximity
- Webhooks
- MCP
trust_url: https://trust.uniqode.com/
---
