---
certification_count: 1
certifications:
- SOC 2 Type I
description: Bruno runs a hosted trust center at trust.usebruno.com and summarises its security posture on its own site at /security. The headline claim is SOC 2 Type I certification, independently audited against the AICPA Trust Services Criteria, with the report, subprocessors and security documentation available through the trust center.
kind: trust-center
layout: security
name: Bruno Api Trust Center
name_suffix: Trust Center
overview: Bruno maintains a public trust center documenting SOC 2 Type I compliance.
provider_name: Bruno
provider_slug: bruno-api
slug: bruno-api-trust-center
source_filename: bruno-api-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nprobe: true\nsource: https://www.usebruno.com/security\nurl: https://trust.usebruno.com\nprovider: Bruno\nproviderId: bruno-api\ndescription: >-\n  Bruno runs a hosted trust center at trust.usebruno.com and summarises its security posture on\n  its own site at /security. The headline claim is SOC 2 Type I certification, independently\n  audited against the AICPA Trust Services Criteria, with the report, subprocessors and security\n  documentation available through the trust center.\ntrust_center:\n  url: https://trust.usebruno.com\n  http_status: 200\n  summary_page: https://www.usebruno.com/security\n  provides: [SOC 2 report, subprocessors, security documentation]\ncertifications:\n- name: SOC 2 Type I\n  status: certified\n  auditor_criteria: AICPA Trust Services Criteria\n  evidence: https://www.usebruno.com/security\nposture:\n  data_residency: >-\n    Local-first - collections, environments and secrets stay on the developer's\
  \ device; Bruno\n    stores no customer API data in a cloud.\n  external_connections: >-\n    Outbound-only HTTPS (TLS 1.2+) on port 443 for licence-key validation and update checks;\n    the licence call sends IP address, licence key, hashed device ID and Bruno version, and no\n    project data. No inbound ports are opened.\n  encryption: TLS 1.2 or higher on all connections.\nevidence:\n- source: https://www.usebruno.com/security\n  http_status: 200\n  keywords: [soc 2 type i, trust center, aicpa trust services criteria, local-first]\n- source: https://trust.usebruno.com\n  http_status: 200\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bruno-api/refs/heads/main/security/bruno-api-trust-center.yml
summary_line: SOC 2 Type I
tags:
- API Client
- API Testing
- Developer Tools
- Open Source
- Git-Native
- CLI
- Postman Alternative
- A2A
- Testing
trust_url: https://trust.usebruno.com
---
