---
certifications:
- ISO 9001:2015
description: ''
kind: trust-center
layout: security
name: Flexgen Power Systems Trust Center
name_suffix: Trust Center
overview: FlexGen Power Systems maintains a public trust center documenting ISO 9001:2015 compliance.
provider_name: FlexGen Power Systems
provider_slug: flexgen-power-systems
slug: flexgen-power-systems-trust-center
source_filename: flexgen-power-systems-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: https://trust.flexgen.com/\ntrust_center:\n  url: https://trust.flexgen.com/\n  http_status: 200\n  title: FlexGen Trust Center\n  platform: Vanta\n  platform_evidence: >-\n    DNS CNAME trust.flexgen.com -> 667f1281bb4f7b57d3bcc51a.cname.vantatrust.com; page assets served\n    from assets.vanta.com; document carries a Vanta trust-report slug (data-slugid).\n  canonical: https://trust.flexgen.com\n  description_meta: >-\n    FlexGen designs and integrates battery energy storage solutions and the software platform that is\n    enabling today's energy transition.\ncertifications:\n- name: ISO 9001:2015\n  scope: >-\n    Design, development, deployment, and remote software support of the HybridOS energy management\n    system software platform.\n  announced: '2026-07-29'\n  evidence: https://www.flexgen.com/resources/blog/flexgens-hybridos-energy-management-system-receives-iso-90012015-certification\n  method: searched\ncertifications_unread:\n\
  \  reason: js-rendered\n  detail: >-\n    The Vanta trust center renders its control/certification list client-side from an authenticated\n    Vanta API. Anonymous GETs of https://trust.flexgen.com/ and every candidate data path return the\n    same 4,367-byte HTML shell; the Vanta GraphQL endpoint rejects unsigned requests\n    (\"Missing `signature` or `signedAt`\") and api.vanta.com/v1 returns 401 Unauthorized. Whatever\n    certifications FlexGen lists inside the trust center could NOT be read without credentials and are\n    therefore NOT recorded here. Absence from this file is not evidence of absence at FlexGen.\n  probes:\n  - url: https://trust.flexgen.com/\n    status: 200\n    content_type: text/html\n  - url: https://app.vanta.com/graphql\n    status: 400\n    note: 'Missing `signature` or `signedAt`'\n  - url: https://api.vanta.com/v1/trust-centers/t4rbw0ujly5ov275f0e77\n    status: 401\nsecurity_contact: null\nvulnerability_disclosure: null\nnote: >-\n  FlexGen serves a real,\
  \ company-branded trust center on its own domain. It publishes no security.txt,\n  no bug-bounty program, and no vulnerability-disclosure policy that could be reached anonymously —\n  see security/flexgen-power-systems-domain-security.yml and well-known/flexgen-power-systems-well-known.yml.\n  No `Security` pointer is emitted, because no disclosure surface was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexgen-power-systems/refs/heads/main/security/flexgen-power-systems-trust-center.yml
summary_line: ISO 9001:2015
tags:
- Company
- Energy
- Energy Storage
- Battery Energy Storage
- Energy Management
- Grid
- Utilities
- Renewable Energy
- Industrial IoT
- SCADA
trust_url: ''
---
