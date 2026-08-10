---
certifications:
- SOC 2 Type II
- ISO/IEC 27001
- ISO/IEC 27017
- ISO/IEC 27018
description: ''
kind: trust-center
layout: security
name: Alcatraz Ai Trust Center
name_suffix: Trust Center
overview: Alcatraz AI maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27017, and ISO/IEC 27018 compliance.
provider_name: Alcatraz AI
provider_slug: alcatraz-ai
slug: alcatraz-ai-trust-center
source_filename: alcatraz-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nprobe: true\nprobe_note: '0-working/probe-security-programs.py returned trust=none — it checks trust./security.\n  subdomains and /trust, /security, /compliance at the apex. Alcatraz AI publishes its\n  trust material one level down, at /resources/privacy-trust-center and /resources/security,\n  which were then fetched and verified by hand.'\nurl: https://www.alcatraz.ai/resources/privacy-trust-center\npages:\n- name: Privacy & Trust Center\n  url: https://www.alcatraz.ai/resources/privacy-trust-center\n- name: Security\n  url: https://www.alcatraz.ai/resources/security\n- name: Responsible AI\n  url: https://www.alcatraz.ai/resources/responsible-ai\n- name: Availability\n  url: https://www.alcatraz.ai/resources/availability\n- name: Rock Privacy Policy\n  url: https://www.alcatraz.ai/utilities/rock-privacy-policy\ncertifications:\n- SOC 2 Type II\n- ISO/IEC 27001\n- ISO/IEC 27017\n- ISO/IEC 27018\ncompliance_programs:\n- GDPR\n- CCPA\n\
  - BIPA\ncontrols:\n- encryption at rest — AES-256 for facial signatures and system data on the Rock\n- encryption in transit — TLS 1.2+\n- edge processing — one-way transform of 3D scans into encrypted data blobs that cannot\n  be reverted to an image; no raw facial image stored or transmitted\n- third-party penetration testing against platform and hardware\n- continuous vulnerability scanning of cloud and edge devices\n- DTAP (development, testing, acceptance, production) firmware release process\n- profiles linked only to an existing badge ID; no name, gender or job title captured\n- auto-deletion of inactive users; opted-out users have no facial data captured\ngaps:\n- No public vulnerability disclosure or bug bounty program; no security.txt (404 on\n  every Alcatraz host probed) and no security@ contact published.\n- No trust portal with downloadable evidence (no Vanta/Drata/SafeBase-style artifact\n  request flow found).\n- The SOC 2 Type II claim on the security page is attributed\
  \ to the underlying AWS\n  infrastructure rather than to an Alcatraz-scoped report; no report identifier or\n  audit period is published.\n- No public status page URL, although the availability page states one is provided\n  to customers.\nx-evidence:\n- url: https://www.alcatraz.ai/resources/security\n  http_status: 200\n  fetched: '2026-08-06'\n  keywords: [soc 2 type ii, iso/iec 27001, iso/iec 27017, iso/iec 27018, aes-256, tls 1.2, penetration test]\n- url: https://www.alcatraz.ai/resources/privacy-trust-center\n  http_status: 200\n  fetched: '2026-08-06'\n  keywords: [gdpr, ccpa, bipa, privacy by design]\n- url: https://www.alcatraz.ai/.well-known/security.txt\n  http_status: 404\n  fetched: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alcatraz-ai/refs/heads/main/security/alcatraz-ai-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018
tags:
- Company
- Access Control
- Biometrics
- Facial Authentication
- Physical Security
- Identity
- Internet of Things
- Artificial Intelligence
trust_url: https://www.alcatraz.ai/resources/privacy-trust-center
---
