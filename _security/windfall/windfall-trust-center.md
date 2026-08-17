---
api_specs:
- filename: windfall-windfall-api-api-openapi.yml
  format: yaml
  label: Windfall Windfall API API
  slug: windfall-windfall-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windfall/refs/heads/main/openapi/windfall-windfall-api-api-openapi.yml
certifications:
- SOC 2 Type 2
- CCPA / California registered data broker
description: ''
kind: trust-center
layout: security
name: Windfall Trust Center
name_suffix: Trust Center
overview: Windfall maintains a public trust center documenting SOC 2 Type 2 and CCPA / California registered data broker compliance.
provider_name: Windfall
provider_slug: windfall
slug: windfall-trust-center
source_filename: windfall-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: false\nurl: https://www.windfall.com/platform/privacy-security\nalso: https://www.windfall.com/security\ncertifications:\n- name: SOC 2 Type 2\n  status: attested\n  continuity: 5 consecutive years\n  evidence: https://www.windfall.com/company/news/windfall-secures-5th-consecutive-soc-2-type-2-certification\n- name: CCPA / California registered data broker\n  status: registered\n  evidence: https://www.windfall.com/platform/privacy-security\nevidence:\n- source: https://www.windfall.com/platform/privacy-security\n  keywords:\n  - soc 2 type 2 compliant\n  - registered data broker in the state of California\n  - fully compliant with CCPA\n- source: https://www.windfall.com/security\n  keywords:\n  - TLS/HTTPS, SFTP, SSL certificates, data encryption\n  - AES 256-bit server-side encryption\n  - OWASP-aligned development standards\n  - intrusion monitoring and data loss prevention\n- source: https://www.windfall.com/company/news/windfall-secures-5th-consecutive-soc-2-type-2-certification\n\
  \  keywords:\n  - 5th consecutive SOC 2 Type 2 certification\ntrust_portal:\n  exists: false\n  probes:\n  - {url: 'https://trust.windfall.com', status: 404}\n  note: >-\n    No dedicated trust portal, evidence room, subprocessor list, or downloadable\n    attestation. Windfall publishes a narrative security page instead; obtaining\n    the SOC 2 report goes through sales.\nvulnerability_disclosure:\n  exists: false\n  security_txt: false\n  bug_bounty: false\n  contact: null\n  probes:\n  - {url: 'https://www.windfall.com/.well-known/security.txt', status: 404}\n  - {url: 'https://windfall.com/.well-known/security.txt', status: 404}\n  - {url: 'https://api-docs.windfall.com/.well-known/security.txt', status: 404}\n  note: >-\n    No responsible-disclosure policy, no security.txt on any host, no\n    HackerOne/Bugcrowd/Intigriti program, and no published security contact\n    address. A researcher who finds a flaw in an API that moves third-party PII\n    has no documented channel. NO\
  \ Security or VulnerabilityDisclosure pointer is\n    wired, because there is no program to point at.\nnot_claimed:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\n- GDPR\nnotes: >-\n  Re-verified 2026-08-14. Windfall's compliance posture is a sustained SOC 2\n  Type 2 program plus statutory California data-broker registration — the latter\n  being the regime that actually governs this API, since the request body is\n  third-party PII and the response is inferred wealth, philanthropy and\n  political-giving data about a natural person.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windfall/refs/heads/main/security/windfall-trust-center.yml
summary_line: SOC 2 Type 2, CCPA / California registered data broker
tags:
- Company
- Fintech
- Data Enrichment
- Wealth Data
- People Intelligence
- Career Data
- Identity Resolution
- Sales Intelligence
- Marketing
trust_url: https://www.windfall.com/platform/privacy-security
---
