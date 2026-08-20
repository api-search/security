---
api_specs:
- filename: termscout-data-openapi.yml
  format: yaml
  label: TermScout Data API
  slug: termscout-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termscout/refs/heads/main/openapi/termscout-data-openapi.yml
certifications:
- SOC 2
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Termscout Trust Center
name_suffix: Trust Center
overview: TermScout maintains a public trust center documenting SOC 2, GDPR, and CCPA compliance.
provider_name: TermScout
provider_slug: termscout
slug: termscout-trust-center
source_filename: termscout-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://security.termscout.com/\nurl: https://security.termscout.com/\nvendor: SafeBase\nvendor_note: >-\n  The trust centre is hosted by SafeBase on TermScout's own subdomain\n  (security.termscout.com). The certifications and documents below are\n  TermScout's; the hosting platform is SafeBase's. Note that the\n  /.well-known/ OAuth and OIDC documents served at this hostname describe\n  SafeBase's own MCP authorization server, NOT a TermScout surface — see\n  well-known/termscout-well-known.yml.\ncertifications:\n- SOC 2\n- GDPR\n- CCPA\ndocuments:\n- Pentest Report\n- Vulnerability Assessment Report\n- Cyber Insurance\nsecurity_contact: infosec@termscout.com\naccess: >-\n  Overview and certification badges are public; the underlying documents are\n  gated behind an NDA/request flow typical of a SafeBase trust centre.\nevidence:\n- source: https://security.termscout.com/\n  http_status: 200\n  fetched: '2026-08-14'\n\
  \  keywords:\n  - soc 2\n  - trust center\n  - gdpr\n  - ccpa\nnote: >-\n  CCPA, the documents list and security_contact were captured by the 2026-07-21\n  search and are retained here. The 2026-08-14 automated re-probe returned a\n  thinner result (SOC 2 + GDPR only, no documents) because the trust centre is a\n  JS-rendered SafeBase application and the keyword probe reads only what is in\n  the served HTML. Retained per the pipeline's idempotency rule — a re-run must\n  not downgrade a richer artifact of equal method.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/termscout/refs/heads/main/security/termscout-trust-center.yml
summary_line: SOC 2, GDPR, CCPA
tags:
- Company
- Legal Tech
- Contract Intelligence
- Contract Certification
- Contract Analysis
- Procurement
- Legal Operations
- Sales Enablement
- Artificial Intelligence
- Contract Data
- Document Analysis
trust_url: https://security.termscout.com/
---
