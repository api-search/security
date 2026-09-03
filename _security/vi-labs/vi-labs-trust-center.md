---
certifications:
- SOC 2 Type 2
- ISO/IEC 27001:2022
- ISO/IEC 27701:2019
- HIPAA
- HITRUST
description: Vi Labs runs a SafeBase-hosted trust center at trust.vi.co (CNAME to vi.portals.safebase.io). It is the company's only published security surface — there is no security.txt, no /security page and no bug bounty program on any Vi Labs host. The portal sits behind a Cloudflare bot challenge, so a plain crawler receives HTTP 403; the page renders for a browser client, and the certifications below were read from that rendered page.
kind: trust-center
layout: security
name: Vi Labs Trust Center
name_suffix: Trust Center
overview: Vi Labs maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001:2022, ISO/IEC 27701:2019, HIPAA, and HITRUST compliance.
provider_name: Vi Labs
provider_slug: vi-labs
slug: vi-labs-trust-center
source_filename: vi-labs-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nprobe: true\nsource: https://trust.vi.co/\nurl: https://trust.vi.co/\nname: Vi Labs Trust Center\ndescription: >-\n  Vi Labs runs a SafeBase-hosted trust center at trust.vi.co (CNAME to\n  vi.portals.safebase.io). It is the company's only published security surface —\n  there is no security.txt, no /security page and no bug bounty program on any\n  Vi Labs host. The portal sits behind a Cloudflare bot challenge, so a plain\n  crawler receives HTTP 403; the page renders for a browser client, and the\n  certifications below were read from that rendered page.\nhost: trust.vi.co\nplatform: SafeBase\ncertifications:\n- SOC 2 Type 2\n- ISO/IEC 27001:2022\n- ISO/IEC 27701:2019\n- HIPAA\n- HITRUST\nsections_observed:\n- App Security\n- Responsible Disclosure\nresponsible_disclosure:\n  referenced: true\n  contact_published: false\n  note: >-\n    The trust center references responsible disclosure, but no contact address\n    or policy URL\
  \ is exposed outside the portal, and no security.txt is served\n    (https://vi.co/.well-known/security.txt -> 404). No VulnerabilityDisclosure\n    artifact or Security pointer is emitted, because nothing publicly resolvable\n    was found.\nevidence:\n- source: https://trust.vi.co/\n  http_status: 403\n  status_note: Cloudflare bot challenge to a plain crawler; page exists and renders for a browser.\n  keywords:\n  - soc 2 type 2\n  - iso/iec 27001:2022\n  - iso/iec 27701:2019\n  - hipaa\n  - hitrust\n  - trust center\n- source: https://vi.co/.well-known/security.txt\n  http_status: 404\n- source: dig trust.vi.co\n  result: vi.portals.safebase.io\nx-evidence:\n  fetched: '2026-09-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vi-labs/refs/heads/main/security/vi-labs-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001:2022, ISO/IEC 27701:2019, HIPAA, HITRUST
tags:
- Company
- Artificial Intelligence
- Health
- Healthcare
- Life Sciences
- Pharmaceuticals
- Patient Engagement
- Enterprise AI
- AI Agents
- Model Context Protocol
- Data
trust_url: https://trust.vi.co/
---
