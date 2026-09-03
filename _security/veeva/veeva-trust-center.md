---
api_specs:
- filename: veeva-authentication-api-openapi.yml
  format: yaml
  label: veeva Authentication API
  slug: veeva-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-authentication-api-openapi.yml
- filename: veeva-documents-api-openapi.yml
  format: yaml
  label: veeva Documents API
  slug: veeva-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-documents-api-openapi.yml
- filename: veeva-objects-api-openapi.yml
  format: yaml
  label: veeva Objects API
  slug: veeva-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-objects-api-openapi.yml
- filename: veeva-query-api-openapi.yml
  format: yaml
  label: veeva Query API
  slug: veeva-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-query-api-openapi.yml
- filename: veeva-users-api-openapi.yml
  format: yaml
  label: veeva Users API
  slug: veeva-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-users-api-openapi.yml
- filename: veeva-workflows-api-openapi.yml
  format: yaml
  label: veeva Workflows API
  slug: veeva-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-workflows-api-openapi.yml
certifications:
- ISO/IEC 27001
- ISO/IEC 27017
- ISO/IEC 27018
- ISO 9001
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Veeva Trust Center
name_suffix: Trust Center
overview: Veeva maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO 9001, and SOC 2 Type II compliance.
provider_name: Veeva
provider_slug: veeva
slug: veeva-trust-center
source_filename: veeva-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://www.veeva.com/trust/\nname: Veeva Security Program Overview\nurl: https://www.veeva.com/trust/\nx-evidence:\n  fetched: '2026-08-15'\n  url: https://www.veeva.com/trust/\n  http_status: 200\n  title: Veeva Security Program Overview | Veeva\ncertifications:\n  - {name: 'ISO/IEC 27001', detail: Information Security Management. Audited at least annually by an accredited third-party certification body.}\n  - {name: 'ISO/IEC 27017', detail: Cloud security controls; covered by the same annual third-party audit.}\n  - {name: 'ISO/IEC 27018', detail: Protection of PII in public clouds; covered by the same annual third-party audit.}\n  - {name: 'ISO 9001', detail: Quality Management Systems.}\n  - {name: 'SOC 2 Type II', detail: System and Organization Controls.}\nframeworks:\n  - SEI Capability Maturity Model Integration (CMMI)\n  - IT Infrastructure Library (ITIL)\n  - 'ICH Q9 — Quality Risk Management'\ncontrols:\n  encryption:\n\
  \    in_transit: 'TLS 1.2 minimum across untrusted networks.'\n    at_rest: 'AES-256 or equivalent.'\n  testing: >-\n    Internal vulnerability testing before every release; internal penetration testing systems;\n    automated and manual vulnerability assessments at least annually; third-party security\n    specialists engaged annually for vulnerability and penetration testing.\n  incident_response: >-\n    Dedicated team operating a formal incident response policy; all personnel trained to report\n    security incidents immediately.\n  access: Documented least-privilege access policies enforced by automated means; separation of duties between operators, admins, and developers.\n  training: Role-based security and annual security awareness training for all employees and contractors.\nstatus_page:\n  url: https://trust.veeva.com/\n  detail: >-\n    Veeva's security overview describes \"a public 'trust' webpage that displays upcoming\n    maintenance downtimes, data center incidents\". Confirmed\
  \ live — see lifecycle/veeva-lifecycle.yml.\ngaps:\n  - No /.well-known/security.txt on any Veeva host (all probes 403/404, 2026-08-15).\n  - No published vulnerability disclosure policy, security contact address, or bug bounty programme found.\n  - No downloadable certificate/report portal; certifications are described in prose rather than served as artifacts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/security/veeva-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO 9001, SOC 2 Type II
tags:
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Regulatory
- Quality Management
- Document-Management
- Content Management
- Healthcare
- Software-as-a-Service
- Enterprise
- MCP
- Agents
trust_url: https://www.veeva.com/trust/
---
