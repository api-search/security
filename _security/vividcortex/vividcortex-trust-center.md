---
api_specs:
- filename: vividcortex-openapi.yml
  format: yaml
  label: VividCortex Database Performance Monitor API
  slug: vividcortex-database-performance-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vividcortex/refs/heads/main/openapi/vividcortex-openapi.yml
certifications:
- SOC 2
- ISO 27001
- GDPR
description: 'VividCortex has no trust center on its own domains (probe 2026-07-21: trust=none on vividcortex.com hosts). As a SolarWinds product (DPM), its compliance posture is published on the SolarWinds Trust Center ("Security Resources", Secure by Design program), which names SOC 2 and ISO/IEC 27001 certifications and GDPR compliance.'
kind: trust-center
layout: security
name: Vividcortex Trust Center
name_suffix: Trust Center
overview: VividCortex maintains a public trust center documenting SOC 2, ISO 27001, and GDPR compliance.
provider_name: VividCortex
provider_slug: vividcortex
slug: vividcortex-trust-center
source_filename: vividcortex-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nurl: https://www.solarwinds.com/trust-center\nsource: https://www.solarwinds.com/trust-center\ndescription: >-\n  VividCortex has no trust center on its own domains (probe 2026-07-21: trust=none on\n  vividcortex.com hosts). As a SolarWinds product (DPM), its compliance posture is\n  published on the SolarWinds Trust Center (\"Security Resources\", Secure by Design\n  program), which names SOC 2 and ISO/IEC 27001 certifications and GDPR compliance.\ncertifications: [SOC 2, ISO 27001, GDPR]\nevidence:\n  - source: https://www.solarwinds.com/trust-center\n    status: 200\n    keywords: [soc 2, iso 27001, iso/iec 27001, gdpr, secure by design]\n    fetched: '2026-07-21'\n  - source: probe-security-programs.py vividcortex\n    kind: probe\n    result: no trust surface on vividcortex.com domains (trust=none)\nnotes:\n  - Trust program is owned by parent company SolarWinds; VividCortex is sold as SolarWinds Database Performance\
  \ Monitor.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vividcortex/refs/heads/main/security/vividcortex-trust-center.yml
summary_line: SOC 2, ISO 27001, GDPR
tags:
- Company
- Database
- Performance Monitoring
- Observability
- Monitoring
- APM
- Database Performance
- SQL
- DevOps
- SolarWinds
trust_url: https://www.solarwinds.com/trust-center
---
