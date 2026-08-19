---
certifications:
- ISO/IEC 27001:2022
- MiCA / CASP licence, AMF No. A2025-008 (granted December 2025)
- Registered DASP (Digital Asset Service Provider)
description: ''
kind: trust-center
layout: security
name: Cometh Trust Center
name_suffix: Trust Center
overview: Cometh maintains a public trust center documenting ISO/IEC 27001:2022, MiCA / CASP licence, AMF No. A2025-008 (granted December 2025), and Registered DASP (Digital Asset Service Provider) compliance.
provider_name: Cometh
provider_slug: cometh
slug: cometh-trust-center
source_filename: cometh-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nurl: https://security.cometh.io/\nplatform: Vanta\nnote: >-\n  Written by hand after probe-security-programs.py reported no hit: the automated probe requires two or more\n  trust/compliance keywords in the response BODY, and this page is a Vanta single-page application whose body is an\n  empty shell (5,005 bytes) that renders its controls, certifications and document list client-side. The hit is real and\n  verified from the shell itself — HTTP 200, `<title>Cometh Trust Center</title>`, `<link rel=\"canonical\"\n  href=\"https://security.cometh.io\">`, Vanta trust-report bundles from assets.vanta.com, and the Vanta slug id\n  4tfjc8kdrwm4rwo3e0wupe. The certification LIST could not be read anonymously (attempts against\n  app.vanta.com/api/trust/<slug> and security.cometh.io/api/* return the same HTML shell; api.vanta.com/v1 returns 401),\n  so the certifications below are attributed to the source that actually states\
  \ them — Kaiko's acquisition announcement\n  — and not to the trust centre.\ncertifications:\n- name: ISO/IEC 27001:2022\n  source: https://kaiko.com/news/Kaiko-Acquires-Cometh-to-Scale-MiCA-Regulated-Onchain-Data-Infrastructure\n  read_from: acquirer announcement (not readable from the trust centre shell)\n- name: MiCA / CASP licence, AMF No. A2025-008 (granted December 2025)\n  source: https://kaiko.com/news/Kaiko-Acquires-Cometh-to-Scale-MiCA-Regulated-Onchain-Data-Infrastructure\n- name: Registered DASP (Digital Asset Service Provider)\n  source: https://cometh.io/\nevidence:\n- source: https://security.cometh.io/\n  http_status: 200\n  content_type: text/html\n  title: Cometh Trust Center\n  body_bytes: 5005\n  keywords: [trust center, vanta]\n  rendering: client-side (JS)\n  vanta_slug_id: 4tfjc8kdrwm4rwo3e0wupe\n- source: https://cometh.io/\n  http_status: 200\n  keywords: [MiCA, DASP, AMF]\n- source: https://kaiko.com/news/Kaiko-Acquires-Cometh-to-Scale-MiCA-Regulated-Onchain-Data-Infrastructure\n\
  \  http_status: 200\n  keywords: [MiCA, CASP, 'AMF No. A2025-008', 'ISO 27001:2022']\ngaps:\n- 'No /.well-known/security.txt on any host (404 on cometh.io/docs/bundler, 401 on paymaster/api.4337).'\n- 'No responsible-disclosure or bug-bounty page found: cometh.io/security, /responsible-disclosure and /vulnerability-disclosure all 404, so no VulnerabilityDisclosure artifact and no Security pointer were written.'\n- 'The trust centre exposes no anonymous machine-readable summary, so certifications cannot be verified from the provider''s own surface without a request through Vanta.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometh/refs/heads/main/security/cometh-trust-center.yml
summary_line: ISO/IEC 27001:2022, MiCA / CASP licence, AMF No. A2025-008 (granted December 2025), Registered DASP (Digital Asset Service Provider)
tags:
- Company
- Blockchain
- account-abstraction
- erc-4337
- smart-wallet
- paymaster
- bundler
- passkeys
- webauthn
- gasless-transactions
- defi
- custody
- staking
- payments
- json-rpc
- mica
- safe
- web3
trust_url: https://security.cometh.io/
---
