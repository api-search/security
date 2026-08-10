---
certifications:
- SOC 2 Type II
- ISO 27001:2013
- ISO 27701
- JOSCAR
- EU-U.S. Data Privacy Framework
- UK Extension to the EU-U.S. Data Privacy Framework
- Swiss-U.S. Data Privacy Framework
description: ''
kind: trust-center
layout: security
name: Red Canary Trust Center
name_suffix: Trust Center
overview: Red Canary maintains a public trust center documenting SOC 2 Type II, ISO 27001:2013, ISO 27701, JOSCAR, EU-U.S. Data Privacy Framework, UK Extension to the EU-U.S. Data Privacy Framework, and Swiss-U.S. Data Privacy Framework compliance.
provider_name: Red Canary
provider_slug: red-canary
slug: red-canary-trust-center
source_filename: red-canary-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nsource: https://redcanary.com/trust-center/\nurls:\n- url: https://redcanary.com/trust-center/\n  kind: marketing trust center page\n- url: https://security.redcanary.com/\n  kind: Conveyor-hosted trust portal (Red Canary Trust Center | Powered by Conveyor)\n  dataroom: https://app.conveyor.com/datarooms/c2853f75-461c-4814-9b4c-5f08fd85b6de\ncontact: grc@redcanary.com\ncertifications:\n- SOC 2 Type II\n- ISO 27001:2013\n- ISO 27701\n- JOSCAR\n- EU-U.S. Data Privacy Framework\n- UK Extension to the EU-U.S. Data Privacy Framework\n- Swiss-U.S. Data Privacy Framework\nprivacy_regimes:\n- GDPR\n- UK GDPR\n- CCPA / CPRA\n- PIPEDA\n- FDPA\nprivacy:\n  dpa: >-\n    Data Protection Addendum available, documenting compliance with GDPR, UK GDPR,\n    CCPA, CPRA, PIPEDA, FDPA and applicable Privacy Acts.\n  privacy_policy: https://redcanary.com/privacy-policy/\nsubprocessors:\n  public: false\n  note: Subprocessor list is available\
  \ to customers and prospects under NDA by request to grc@redcanary.com.\nvulnerability_disclosure: https://redcanary.com/responsible-disclosure/\nstatus_page: https://status.redcanary.com/\ncustomer_compliance_support:\n  url: https://docs.redcanary.com/docs/supported-standards-and-frameworks\n  note: >-\n    Control-family mappings showing how Red Canary monitoring supports CUSTOMER\n    obligations under ISO 27001:2013, SOC, FedRAMP, PCI DSS, BSI C5, HIPAA,\n    NIST 800-171 and CMMC. These are frameworks Red Canary helps customers satisfy —\n    they are NOT certifications Red Canary itself holds, and must not be read as such.\nx-false-credit-guard: >-\n  The automated probe (0-working/probe-security-programs.py) first recorded HIPAA,\n  FedRAMP, ISO 27017, ISO 27018 and CSA STAR from https://security.redcanary.com/.\n  Those strings are real on that page but belong to OTHER vendors' tiles rendered in\n  the Conveyor portal's directory carousel (Slack, Zendesk, Splunk, AWS). Red Canary's\n\
  \  own record in the page's VENDOR_REPORT payload lists exactly:\n  [\"iso-27001\",\"iso-27701\",\"soc2-type-2\",\"ccpa\",\"eu-us-data-privacy\",\"gdpr\",\n  \"swiss-us-dpf\",\"uk-extension-to-eu-us-dpf\"], which matches the marketing trust center\n  page. The keyword-derived list was discarded and this file was restored to the\n  searched values. Do not re-run the probe over this file without re-verifying.\nevidence:\n- source: https://redcanary.com/trust-center/\n  http_status: 200\n  keywords:\n  - soc 2 type ii\n  - iso 27001:2013\n  - iso 27701\n  - joscar\n  - data privacy framework\n- source: https://security.redcanary.com/\n  http_status: 200\n  extracted: window.VENDOR_REPORT._embedded.canonical_asset.certifications\n  value:\n  - iso-27001\n  - iso-27701\n  - soc2-type-2\n  - ccpa\n  - eu-us-data-privacy\n  - gdpr\n  - swiss-us-dpf\n  - uk-extension-to-eu-us-dpf\n- source: https://redcanary.com/security/\n  http_status: 200\n  note: 301 to https://redcanary.com/trust-center/\n\
  - source: https://trust.redcanary.com/\n  http_status: 0\n  note: does not resolve\nx-evidence:\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-canary/refs/heads/main/security/red-canary-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001:2013, ISO 27701, JOSCAR, EU-U.S. Data Privacy Framework, UK Extension to the EU-U.S. Data Privacy Framework, Swiss-U.S. Data Privacy Framework
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Threat Detection
- Threat Intelligence
- Endpoint Security
- Incident Response
- Security Operations
- Automation
trust_url: ''
---
