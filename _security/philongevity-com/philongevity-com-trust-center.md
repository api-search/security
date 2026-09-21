---
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Philongevity Com Trust Center
name_suffix: Trust Center
overview: Phi Longevity maintains a public trust center covering its security and compliance posture.
provider_name: Phi Longevity
provider_slug: philongevity-com
slug: philongevity-com-trust-center
source_filename: philongevity-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nurl: https://philongevity.com/trust\ntitle: Trust & Data Stewardship\nlast_updated: '2026-08-20'\ncertifications: []\ncompliance_claims:\n- claim: HIPAA-eligible storage under a signed Google Cloud HIPAA Business Associate Agreement (Firestore, Cloud Healthcare API FHIR store, Cloud Storage); analysis on US-pinned Vertex AI under the same agreement\n  source: https://philongevity.com/trust\n- claim: HIPAA Alignment Statement — administrative, physical and technical safeguards consistent with the HIPAA Security Rule; not a covered entity\n  source: https://philongevity.com/privacy\n- claim: Encryption in transit TLS 1.2+, at rest AES-256; role-based access; audit logs of administrative data access\n  source: https://philongevity.com/privacy\n- claim: Health data not used to train AI models; not sold; aggregate-only telemetry (counts, booleans, timings — no values, filenames or identifiers)\n  source: https://philongevity.com/trust\n\
  - claim: Account deletion is a single authoritative purge across Firestore, the FHIR store, Cloud Storage, exports and the auth record; full data export on request\n  source: https://philongevity.com/trust\n- claim: Agent surfaces (MCP, A2A) accept synthetic or de-identified inputs only; PHI never transits them — \"the boundary is architectural, not procedural\"; agent identity verifiable via ES256-signed card and /.well-known/jwks.json\n  source: https://philongevity.com/trust\ninherited_not_own:\n- Google Cloud SOC 2 Type II and ISO 27001 are cited on /privacy — these are the infrastructure provider's certifications, not an audit of Phi Longevity, so certifications[] above is empty.\ncontact: support@philongevity.com\nevidence:\n- {source: 'https://philongevity.com/trust', http_status: 200, keywords: [HIPAA, Business Associate Agreement, encryption, deletion, export, telemetry, agent identity]}\n- {source: 'https://philongevity.com/privacy', http_status: 200, keywords: [HIPAA Alignment\
  \ Statement, AES-256, TLS 1.2, SOC 2 Type II (Google Cloud), ISO 27001 (Google Cloud)]}\nnote: probe-security-programs.py recorded trust=none for this host because /trust did not clear its keyword bar; the page is nonetheless a dedicated, dated trust page carrying a HIPAA BAA posture statement, so it is recorded here by hand with the certifications list left honestly empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philongevity-com/refs/heads/main/security/philongevity-com-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Health Data
- Lab Results
- Biomarkers
- Chronic Disease
- Longevity
- MCP
- A2A
- Agent Payments
- x402
- Artificial Intelligence
trust_url: https://philongevity.com/trust
---
