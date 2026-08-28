---
api_specs:
- filename: relex-data-api-openapi.json
  format: json
  label: RELEX Data API
  slug: relex-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-data-api-openapi.json
- filename: relex-monitoring-api-openapi.json
  format: json
  label: RELEX Monitoring API
  slug: relex-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-monitoring-api-openapi.json
certifications:
- ISO/IEC 27001:2013
- SOC 2 (ISAE 3000)
- GDPR
description: ''
kind: trust-center
layout: security
name: Relex Trust Center
name_suffix: Trust Center
overview: RELEX Solutions maintains a public trust center documenting ISO/IEC 27001:2013, SOC 2 (ISAE 3000), and GDPR compliance.
provider_name: RELEX Solutions
provider_slug: relex
slug: relex-trust-center
source_filename: relex-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nprobe: true\nsource: https://www.relexsolutions.com/security-compliance/\nurl: https://www.relexsolutions.com/privacy-trust-center/\nhttp_status: 200\ntrust_center:\n  present: true\n  style: static policy pages, not a hosted trust portal\n  note: >-\n    RELEX runs no Vanta/Drata/SafeBase-style trust portal with downloadable, gated evidence. What\n    it publishes is a set of readable policy pages. Audit reports themselves (the SOC 2 report,\n    the ISO certificate) are not downloadable and are presumably obtained through sales or the\n    customer relationship.\n  pages:\n  - name: Security and compliance\n    url: https://www.relexsolutions.com/security-compliance/\n    status: 200\n  - name: Privacy trust center\n    url: https://www.relexsolutions.com/privacy-trust-center/\n    status: 200\n  - name: Information security FAQ\n    url: https://www.relexsolutions.com/policy/infosec-faq/\n    status: 200\n  - name: AI governance\
  \ and trust at RELEX\n    url: https://www.relexsolutions.com/policy/ai-governance-trust-at-relex/\n    status: 200\n  - name: Vulnerability disclosure policy\n    url: https://www.relexsolutions.com/policy/vulnerability-disclosure/\n    status: 200\n  - name: Modern slavery statement\n    url: https://www.relexsolutions.com/policy/modern-slavery-statement/\n  - name: Whistleblowing channel\n    url: https://www.relexsolutions.com/policy/whistleblowing-channel/\ncertifications:\n- name: ISO/IEC 27001:2013\n  scope: RELEX Inventory and Supply Chain software\n  evidence: 'Named on the security and compliance page: \"To gain ISO 27001:2013 certification for\n    RELEX''s Inventory and Supply Chain software, we had to demonstrate a systematic and rigorous\n    approach to managing sensitive information.\"'\n  certificate_downloadable: false\n- name: SOC 2 (ISAE 3000)\n  detail: Type I and Type II reports completed\n  evidence: RELEX describes the ISAE 3000 SOC 2 standard as its assurance reporting\
  \ standard and\n    states both Type I and Type II reports are complete.\n  report_downloadable: false\n- name: GDPR\n  detail: EU data protection programme\n  evidence: Named on the security and compliance page; RELEX is Helsinki-headquartered and offers\n    EU-resident environments (uat-eu / eu API hosts, identity.prod-eu identity authority).\n  note: A regulatory obligation rather than a certification, but published as part of the same\n    programme.\nnot_found:\n- PCI DSS\n- HIPAA\n- FedRAMP\n- ISO 27017\n- ISO 27018\n- ISO 27701\n- TISAX\n- CSA STAR\nsubprocessors:\n  published: false\n  note: >-\n    No subprocessor list was found, though at least two subprocessors are inferable from the API\n    documentation itself — Svix (webhook delivery) and Microsoft Azure (Blob Storage for the Batch\n    API; the developer portal runs on Azure Static Web Apps).\ndata_residency:\n  regions:\n  - eu\n  - us\n  evidence: Both APIs publish per-region hosts and per-region RELEX Identity authorities,\
  \ so\n    residency is selectable at the environment level.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/security/relex-trust-center.yml
summary_line: ISO/IEC 27001:2013, SOC 2 (ISAE 3000), GDPR
tags:
- Supply Chain
- Retail
- Demand Planning
- Inventory Management
- Forecasting
- Pricing
- Enterprise Software
- Data Integration
- Company
trust_url: https://www.relexsolutions.com/privacy-trust-center/
---
