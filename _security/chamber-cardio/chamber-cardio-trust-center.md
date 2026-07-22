---
certifications:
- SOC 2
- HIPAA
- ONC
description: Chamber Cardio operates a live, Vanta-hosted Trust Center at trust.chambercardio.com/controls. The trust center page is JavaScript-rendered (Vanta SPA), so the automated security-programs probe could not extract the named certification list from its HTML; the trust center itself was verified live (HTTP 200, canonical Vanta trust-report shell). The certifications below are captured from the published Medplum engineering case study, which states Chamber's platform has SOC 2, HIPAA, and ONC compliance built in. Treat the live Vanta trust center as the authoritative, current source of record.
kind: trust-center
layout: security
name: Chamber Cardio Trust Center
name_suffix: Trust Center
overview: Chamber Cardio maintains a public trust center documenting SOC 2, HIPAA, and ONC compliance.
provider_name: Chamber Cardio
provider_slug: chamber-cardio
slug: chamber-cardio-trust-center
source_filename: chamber-cardio-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: true\nsource: https://trust.chambercardio.com\nurl: https://trust.chambercardio.com\nplatform: Vanta Trust Center\ndescription: >-\n  Chamber Cardio operates a live, Vanta-hosted Trust Center at\n  trust.chambercardio.com/controls. The trust center page is JavaScript-rendered\n  (Vanta SPA), so the automated security-programs probe could not extract the\n  named certification list from its HTML; the trust center itself was verified\n  live (HTTP 200, canonical Vanta trust-report shell). The certifications below\n  are captured from the published Medplum engineering case study, which states\n  Chamber's platform has SOC 2, HIPAA, and ONC compliance built in. Treat the\n  live Vanta trust center as the authoritative, current source of record.\ncertifications:\n  - {name: SOC 2, source: 'https://www.medplum.com/blog/chamber-cardio-case-study'}\n  - {name: HIPAA, source: 'https://www.medplum.com/blog/chamber-cardio-case-study'}\n\
  \  - {name: ONC, note: ONC Health IT certification, source: 'https://www.medplum.com/blog/chamber-cardio-case-study'}\nevidence:\n  - {source: https://trust.chambercardio.com, kind: trust-center, note: 'Live Vanta trust center (HTTP 200), certifications not machine-extractable from JS shell'}\n  - {source: https://www.medplum.com/blog/chamber-cardio-case-study, kind: case-study, keywords: [soc 2, hipaa, onc, compliant]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chamber-cardio/refs/heads/main/security/chamber-cardio-trust-center.yml
summary_line: SOC 2, HIPAA, ONC
tags:
- Company
- Healthcare
- Cardiology
- Value-Based Care
- Health Tech
- FHIR
- Care Coordination
- Payers
trust_url: https://trust.chambercardio.com
---
