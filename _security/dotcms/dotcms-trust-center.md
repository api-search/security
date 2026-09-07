---
api_specs:
- filename: dotcms-rest-api-openapi.json
  format: json
  label: dotCMS REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/openapi/dotcms-rest-api-openapi.json
certification_count: 5
certifications:
- ISO/IEC 27001:2022
- ISO/IEC 42001:2023
- SOC 2 Type II
- TX-RAMP Level II
- CSA CAIQ
description: dotCMS runs a hosted trust center at security.dotcms.com carrying its certifications, the CAIQ and a gated SOC 2 report request. The public summary page at /product/security-compliance names the certifications outright, so they are recorded here from the provider's own words rather than inferred from a badge image.
kind: trust-center
layout: security
name: Dotcms Trust Center
name_suffix: Trust Center
overview: dotCMS maintains a public trust center documenting ISO/IEC 27001:2022, ISO/IEC 42001:2023, SOC 2 Type II, TX-RAMP Level II, and CSA CAIQ compliance.
provider_name: dotCMS
provider_slug: dotcms
slug: dotcms-trust-center
source_filename: dotcms-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprobe: true\nurl: https://security.dotcms.com/\npublic_summary: https://www.dotcms.com/product/security-compliance\ndescription: >-\n  dotCMS runs a hosted trust center at security.dotcms.com carrying its certifications, the CAIQ\n  and a gated SOC 2 report request. The public summary page at /product/security-compliance\n  names the certifications outright, so they are recorded here from the provider's own words\n  rather than inferred from a badge image.\ncertifications:\n- ISO/IEC 27001:2022\n- ISO/IEC 42001:2023\n- SOC 2 Type II\n- TX-RAMP Level II\n- CSA CAIQ\ndocuments:\n- name: SOC 2 Type II report\n  access: request\n  url: https://security.dotcms.com/?requestAccessOpen=true&requestedResources=68bf49dffa149b0f145d21eb\n  note: Gated behind an access request, which is normal for a SOC 2 Type II report.\n- name: CAIQ (Consensus Assessments Initiative Questionnaire)\n  access: public\n  url: https://security.dotcms.com/doc/trust?rid=65ea66456af50d8aa7bb69bc&r=2sr38oqu8xcq3f7qdsuhn\n\
  positioning: >-\n  Compliance is dotCMS's stated market position, not a footnote — the homepage title is\n  \"Visual Headless CMS for Compliance-led Enterprises\" and the security page frames governance as\n  \"enforced by the platform, not configured per site\". ISO/IEC 42001 is the notable one: dotCMS\n  extends its AI governance claim to agent behaviour, describing an AI agent as \"another actor in\n  the system: it works inside the same roles, permissions, and workflows as a person, and every\n  change it makes stays traceable and reversible through version history\" — a claim that lines up\n  with the reversibility surface recorded in conventions/dotcms-conventions.yml.\nevidence:\n- source: https://security.dotcms.com/\n  status: 200\n  kind: trust center\n- source: https://www.dotcms.com/product/security-compliance\n  status: 200\n  keywords: [iso 27001, iso 42001, soc 2 type ii, tx-ramp, caiq, trust center]\n- source: https://www.dotcms.com/.well-known/security.txt\n  status: 200\n\
  \  kind: security.txt\nchecked: '2026-09-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/security/dotcms-trust-center.yml
summary_line: ISO/IEC 27001:2022, ISO/IEC 42001:2023, SOC 2 Type II, TX-RAMP Level II, CSA CAIQ
tags:
- CMS
- Content
- Content Management
- Headless CMS
- Digital Experience
- Content Delivery
- Workflows
- GraphQL
- MCP
- Java
trust_url: https://security.dotcms.com/
---
