---
api_specs:
- filename: optilogic-rest-api-openapi.json
  format: json
  label: Optilogic REST API
  slug: optilogic-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-rest-api-openapi.json
certifications:
- SOC 2 Type II
- CMMC Level 1
description: ''
kind: trust-center
layout: security
name: Optilogic Trust Center
name_suffix: Trust Center
overview: Optilogic maintains a public trust center documenting SOC 2 Type II and CMMC Level 1 compliance.
provider_name: Optilogic
provider_slug: optilogic
slug: optilogic-trust-center
source_filename: optilogic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nprobe: true\nsource: https://trust.optilogic.com/\nurl: https://trust.optilogic.com/\ncertifications:\n- SOC 2 Type II\n- CMMC Level 1\nevidence:\n- source: https://trust.optilogic.com/\n  keywords:\n  - soc 2 type ii\n  - cmmc level 1\n  - trust center\n  - safebase\nplatform: SafeBase\ncertification_detail:\n- name: SOC 2 Type II\n  status: completed\n  as_of: 2025-05\n  evidence: '\"As of May, 2025, Optilogic has successfully completed SOC 2 Type II.\" (trust.optilogic.com)'\n- name: CMMC Level 1\n  status: held\n  framework: NIST 800-171/172, US Department of Defense\n  evidence: Trust center states CMMC Level 1 and that Optilogic is \"continuing to harden its cybersecurity\n    posture by proceeding to implement CMMC Level 2 compliance.\"\n- name: CMMC Level 2\n  status: in-progress\n  evidence: Stated as in implementation on the trust center; not yet held.\ndocuments_gated:\n- SOC 2 Report\n- Data Flow Diagram (DFD)\n- Web App\
  \ Pentest Report\n- CMMC Certification documentation\nsecurity_contact: opti-infosec@optilogic.com\naccess: The trust center index is public. The underlying reports (SOC 2, pentest, DFD) are request-gated\n  behind the SafeBase portal.\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://trust.optilogic.com/\n  http_status_direct_curl: 403\n  note: A direct curl with a browser User-Agent is answered 403 by the SafeBase edge (bot challenge, 5,730-byte\n    body). The page demonstrably exists and renders for an ordinary client; the certification detail above\n    was read from the rendered page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/security/optilogic-trust-center.yml
summary_line: SOC 2 Type II, CMMC Level 1
tags:
- Supply Chain
- Supply Chain Design
- Network Optimization
- Simulation
- Optimization
- Logistics
- Analytics
- Artificial Intelligence
- Jobs
- Cloud
trust_url: https://trust.optilogic.com/
---
