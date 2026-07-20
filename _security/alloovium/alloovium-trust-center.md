---
api_specs:
- filename: openapi.json
  format: json
  label: Alloovium API
  slug: alloovium-api
  spec_type: OpenAPI
  url: https://api.alloovium.com/api/v2/openapi.json
certifications:
- SOC 2 Type I
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Alloovium Trust Center
name_suffix: Trust Center
overview: Alloovium maintains a public trust center documenting SOC 2 Type I and ISO 27001 compliance.
provider_name: Alloovium
provider_slug: alloovium
slug: alloovium-trust-center
source_filename: alloovium-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nprobe: false\nurl: https://www.alloovium.com/en/security\ncompliance_manager: Vanta\ncertifications:\n- {name: SOC 2 Type I, status: in-progress}\n- {name: ISO 27001, status: in-progress}\nencryption:\n  at_rest: Documents in AWS S3 with KMS encryption; PostgreSQL via RDS encryption.\n  in_transit: TLS 1.2 or higher enforced on all connections.\n  enterprise: BYOK (Bring Your Own Key) available.\ndata_residency:\n  primary: AWS ap-southeast-2 (Sydney, Australia)\n  note: Document storage and databases remain in-region.\nsecurity_scanning: Dependabot enabled; zero security incidents reported to date.\nsecurity_contact: zander@alloovium.com\nevidence:\n- {source: https://www.alloovium.com/en/security, keywords: [soc 2, iso 27001, vanta, kms, tls, byok, data residency]}\nnotes: >-\n  Named certifications are recorded as in-progress (not yet achieved), managed via Vanta. Reported honestly;\n  no Compliance pointer is emitted since no certification\
  \ is completed as of this pass.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloovium/refs/heads/main/security/alloovium-trust-center.yml
summary_line: SOC 2 Type I, ISO 27001
tags:
- Company
- Construction
- Document Intelligence
- Compliance
- Artificial Intelligence
- Construction Technology
- Documents
- MCP
trust_url: https://www.alloovium.com/en/security
---
