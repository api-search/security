---
api_specs:
- filename: zyte-zyte-api-openapi.yaml
  format: yaml
  label: Zyte API
  slug: zyte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zyte/refs/heads/main/openapi/zyte-zyte-api-openapi.yaml
- filename: zyte-stats-api-openapi.yaml
  format: yaml
  label: Zyte API Stats API
  slug: zyte-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zyte/refs/heads/main/openapi/zyte-stats-api-openapi.yaml
certifications:
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Zyte Trust Center
name_suffix: Trust Center
overview: Zyte maintains a public trust center documenting ISO 27001 compliance.
provider_name: Zyte
provider_slug: zyte
slug: zyte-trust-center
source_filename: zyte-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://www.zyte.com/trust-center/\nprovider: Zyte\nproviderId: zyte\ntrust_center:\n  name: Zyte Security Trust Center\n  url: https://www.zyte.com/trust-center/\n  http_status: 200\n  platform: self-hosted\n  note: >-\n    A page on the marketing site, not a Vanta/Drata/SafeBase hosted trust\n    portal. There is no machine-readable feed and no document-request workflow\n    beyond email/sales contact.\ncertifications:\n  - name: ISO 27001\n    status: certified\n    scope: Zyte itself, and Zyte states all of its hosting providers are also ISO 27001 certified.\n    certifier_reference: https://isoqar.com/iso-standards/iso-27001/\n    evidence: >-\n      \"Zyte is ISO 27001 certified and all of its hosting providers have\n      achieved ISO 27001 certification.\"\ncompliance:\n  - name: GDPR\n    status: claimed\n    evidence: >-\n      \"Zyte is committed to GDPR compliance. We have implemented robust data\n      protection...\"\
  \n  - name: CCPA\n    status: claimed\n  - name: FISD Alternative Data Standards\n    status: co-author\n    note: >-\n      Zyte states it co-authored the FISD Alternative Data Standards — a\n      domain-relevant standard for the alternative-data market Zyte sells into.\n      Recorded also in conformance/zyte-conformance.yml.\nabsent:\n  - name: SOC 2\n    note: >-\n      Not claimed on the trust center. NOTE: https://www.zyte.com/security-and-compliance/\n      returns HTTP 200 but is a soft-404 shell byte-identical to a nonsense slug —\n      the compliance content lives only at /trust-center/.\n  - name: PCI DSS\n    note: Not claimed; Zyte does not handle cardholder data on behalf of customers.\n  - name: HIPAA\n    note: Not claimed.\n  - name: FedRAMP\n    note: Not claimed.\npenetration_testing:\n  performed: true\n  report_availability: on request\n  evidence: >-\n    \"Zyte can provide penetration test reports to clients upon request. To\n    ensure the confidentiality and\
  \ security of sensitive information, access to\n    these reports [is restricted].\"\ndata_processing:\n  dpa: https://www.zyte.com/terms-policies/dpa/\n  subprocessors: https://www.zyte.com/terms-policies/subprocessor/\n  subprocessor_list_location: Annex III of the Data Processing Agreement\n  privacy_policy: https://www.zyte.com/terms-policies/privacy-policy/\n  do_not_sell: https://www.zyte.com/terms-policies/do-not-sell/\n  acceptable_use: https://www.zyte.com/terms-policies/acceptable-use-policy/\nrelated:\n  - security/zyte-vulnerability-disclosure.yml\n  - security/zyte-domain-security.yml\n  - conformance/zyte-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zyte/refs/heads/main/security/zyte-trust-center.yml
summary_line: ISO 27001
tags:
- Crawling
- Data Extraction
- Scraping
- Web Scraping
- Proxies
- Browser Automation
- Anti-Ban
- SERP
- Agent Skills
- Developer Tools
trust_url: ''
---
