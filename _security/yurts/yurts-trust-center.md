---
certification_count: 9
certifications:
- SOC 2 Type 2
- SOC 1 Type 2
- FedRAMP High
- CMMC Level 2
- NIST 800-53
- HIPAA
- GDPR
- ITAR
- DoD Impact Level IL2-IL6
description: ''
kind: trust-center
layout: security
name: Yurts Trust Center
name_suffix: Trust Center
overview: Yurts maintains a public trust center documenting SOC 2 Type 2, SOC 1 Type 2, FedRAMP High, CMMC Level 2, NIST 800-53, HIPAA, GDPR, ITAR, and DoD Impact Level IL2-IL6 compliance.
provider_name: Yurts
provider_slug: yurts
slug: yurts-trust-center
source_filename: yurts-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nprobe: true\nsource: https://www.legionintel.com/security\nurl: https://www.legionintel.com/security\nnote: >-\n  Yurts rebranded to Legion Intelligence, Inc.; the security and compliance page is published on the\n  successor domain. A dedicated hosted trust center is provisioned at https://trust.legionintel.com/\n  and https://trust.yurts.ai/ — both CNAME to trust.cname.drata.com (Drata Trust Center), and both\n  answered our probe with a Cloudflare interstitial (\"Just a moment...\", HTTP 403) rather than the\n  page, so the certification list below is read from the first-party /security page and the\n  company's own llms.txt, not from the Drata portal.\ntrust_centers:\n- url: https://trust.legionintel.com/\n  platform: Drata\n  evidence: DNS CNAME trust.legionintel.com -> trust.cname.drata.com\n  http_status: 403\n  http_status_note: Cloudflare bot challenge, not a dead page\n- url: https://trust.yurts.ai/\n  platform: Drata\n \
  \ evidence: DNS CNAME trust.yurts.ai -> trust.cname.drata.com\n  http_status: 403\n  http_status_note: legacy brand host, same Drata target\ncertifications:\n- name: SOC 2 Type 2\n  evidence: https://www.legionintel.com/security\n- name: SOC 1 Type 2\n  evidence: https://www.legionintel.com/security\n- name: FedRAMP High\n  scope: cloud platform\n  evidence: https://www.legionintel.com/llms.txt\n- name: CMMC Level 2\n  evidence: https://www.legionintel.com/llms.txt\n- name: NIST 800-53\n  evidence: https://www.legionintel.com/llms.txt\n- name: HIPAA\n  kind: attestation\n  evidence: https://www.legionintel.com/security\n- name: GDPR\n  kind: attestation\n  evidence: https://www.legionintel.com/security\n- name: ITAR\n  kind: readiness\n  note: stated as \"ready to manage ITAR-controlled data\"\n  evidence: https://www.legionintel.com/llms.txt\n- name: DoD Impact Level IL2-IL6\n  kind: authorization range\n  evidence: https://www.legionintel.com/security\nsupply_chain:\n- artifact: SBOM\n\
  \  evidence: https://www.legionintel.com/llms.txt\n- artifact: HBOM\n  evidence: https://www.legionintel.com/llms.txt\nevidence:\n- source: https://www.legionintel.com/security\n  http_status: 200\n  keywords:\n  - soc 1 type 2\n  - soc 2 type 2\n  - hipaa\n  - gdpr\n  - cmmc\n  - fedramp high\n  - il2-6\n- source: https://www.legionintel.com/llms.txt\n  http_status: 200\n  keywords:\n  - fedramp high\n  - nist 800-53\n  - soc 2 type ii\n  - cmmc level 2\n  - itar\n  - hbom/sbom\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yurts/refs/heads/main/security/yurts-trust-center.yml
summary_line: SOC 2 Type 2, SOC 1 Type 2, FedRAMP High, CMMC Level 2, NIST 800-53, HIPAA, GDPR, ITAR, DoD Impact Level IL2-IL6
tags:
- Company
- Artificial Intelligence
- Agentic AI
- National Security
- Defense
- Generative AI
- Enterprise Search
- Retrieval Augmented Generation
- Edge AI
- Government
trust_url: https://www.legionintel.com/security
---
