---
api_specs:
- filename: mercury-hq-com-x402-storefront-openapi.yml
  format: yaml
  label: MERCURY x402 Storefront API
  slug: mercury-x402-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/openapi/mercury-hq-com-x402-storefront-openapi.yml
certification_count: 0
certifications: []
description: MERCURY publishes a trust page ("Trust & reputability - what a procurement buyer, a directory, or a skeptical agent needs before transacting") that is an operator-identity and verify-it-yourself page rather than a certification portal. It names the operator (Mercury Holdings Pty Ltd, an Australian Pty Ltd with ASIC registration in progress - "ABN/ACN published here ONLY once issued"; jurisdiction Queensland; governance "Mercury Foundation - standards & governance arm ... NOT a token foundation"; contact mercuryuser@proton.me with https://mercury-x402-jed.fly.dev as fallback), the three things a reader can verify independently (offline EIP-191 receipt verification against the pinned key, USDC settlement on a public chain via the payTo wallet on BaseScan, and catalog/checkout generated from one object so they cannot drift), and a "what we do NOT do" list (no token, no faked traction - "N=0 external buyers and $0 external revenue today", no payload retention - "we do not store,
  resell, or train on the content you fetch"). It names NO SOC 2, ISO 27001, PCI DSS, HIPAA, GDPR or other certification or audit, so no Compliance pointer is emitted. probe-security-programs.py did not record it because the page carries fewer than two of the keywords it requires; it is recorded here by hand because the page is real, first-party and answers the trust question directly.
kind: trust-center
layout: security
name: Mercury Hq Com Trust Center
name_suffix: Trust Center
overview: MERCURY maintains a public trust center covering its security and compliance posture.
provider_name: MERCURY
provider_slug: mercury-hq-com
slug: mercury-hq-com-trust-center
source_filename: mercury-hq-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nurl: https://network.mercury-hq.com/trust\ncertifications: []\ndescription: >-\n  MERCURY publishes a trust page (\"Trust & reputability - what a procurement buyer, a directory, or a\n  skeptical agent needs before transacting\") that is an operator-identity and verify-it-yourself page\n  rather than a certification portal. It names the operator (Mercury Holdings Pty Ltd, an Australian Pty\n  Ltd with ASIC registration in progress - \"ABN/ACN published here ONLY once issued\"; jurisdiction\n  Queensland; governance \"Mercury Foundation - standards & governance arm ... NOT a token foundation\";\n  contact mercuryuser@proton.me with https://mercury-x402-jed.fly.dev as fallback), the three things a\n  reader can verify independently (offline EIP-191 receipt verification against the pinned key, USDC\n  settlement on a public chain via the payTo wallet on BaseScan, and catalog/checkout generated from one\n  object so they cannot\
  \ drift), and a \"what we do NOT do\" list (no token, no faked traction - \"N=0 external\n  buyers and $0 external revenue today\", no payload retention - \"we do not store, resell, or train on the\n  content you fetch\"). It names NO SOC 2, ISO 27001, PCI DSS, HIPAA, GDPR or other certification or audit,\n  so no Compliance pointer is emitted. probe-security-programs.py did not record it because the page\n  carries fewer than two of the keywords it requires; it is recorded here by hand because the page is\n  real, first-party and answers the trust question directly.\noperator:\n  legal_name: Mercury Holdings Pty Ltd\n  type: Australian proprietary limited company (Pty Ltd)\n  registration: in progress (ASIC); no ABN/ACN published\n  jurisdiction: Queensland, Australia\n  governance: Mercury Foundation (standards and governance arm; no token)\n  contact: mercuryuser@proton.me\nverifiable_claims:\n- {claim: signed provenance receipts, how: 'EIP-191 ecrecover over sha256(content)‖url‖status‖fetchedAt‖nonce\
  \ against the pinned key 0xACB40253BD71Bb9a5d491b2c6EFF755F2A33Fc75 (/.well-known/mercury-attestation); verifier at /x402/verify'}\n- {claim: on-chain settlement, how: 'shop wallet 0xe10B9d44e72A29B9c19da02981FFCd875308e3C1 on BaseScan; CDP facilitator; /treasury page shows live balances and $0.00 external earnings'}\n- {claim: catalog cannot drift from checkout, how: '/catalog, /openapi.json, /.well-known/x402 and the live 402 are generated from the same catalog object (checked: the 402 for /buy/fetch carried maxAmountRequired 3000, matching $0.003 in all three documents)'}\ndata_handling:\n  payload_retention: none stated (\"We do not retain fetched content beyond returning it in the response\"; /privacy)\n  logs: minimal operational logs (timestamp, route, status)\n  personal_data: '\"We do not ask for or collect personal information\" (/privacy, last updated 2026-06-04)'\nrelated_pages:\n- {url: 'https://network.mercury-hq.com/terms', status: 200, note: 'terms effective 2026-06-04;\
  \ machine-readable with Accept: application/json'}\n- {url: 'https://network.mercury-hq.com/privacy', status: 200}\n- {url: 'https://network.mercury-hq.com/university/treasury', status: 200, note: live wallet balances and revenue (all external figures $0.00)}\n- {url: 'https://network.mercury-hq.com/proof', status: 200, note: 'x402 self-settlement proof: \"no on-chain settlement recorded yet\"'}\n- {url: 'https://network.mercury-hq.com/reviews', status: 200, note: ERC-8004 on-chain reviews page (wallet-connect UI)}\nevidence:\n- {source: 'https://network.mercury-hq.com/trust', status: 200, keywords: [trust, reputability, operator, verify, no payload retention, jurisdiction]}\nprobed_absent:\n- {url: 'https://trust.mercury-hq.com/', status: 'no DNS'}\n- {url: 'https://mercury-hq.com/trust', status: 404}\n- {url: 'https://network.mercury-hq.com/security', status: 404}\n- {url: 'https://network.mercury-hq.com/compliance', status: 'not probed - no link to it anywhere'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/security/mercury-hq-com-trust-center.yml
summary_line: trust center published
tags:
- Company
- Agents
- A2A
- MCP
- x402
- HTTP 402
- Machine Payments
- Web Data
- Web Scraping
- Data Extraction
- Provenance
- Stablecoins
- Artificial Intelligence
trust_url: https://network.mercury-hq.com/trust
---
