---
api_specs:
- filename: alphaai-rest-api-openapi.yml
  format: yaml
  label: AlphaAI REST API
  slug: alphaai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/openapi/alphaai-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: alphai.io
  spf: true
  spf_record: v=spf1 include:zohomail.com ~all
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: alphai.io
  hsts: false
  https: true
  note: Next.js behind CloudFront. Serves CSP frame-ancestors 'none' and X-Frame-Options DENY, but no Strict-Transport-Security on the marketing host — the one host most likely to be typed into a browser bar.
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: api.alphai.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: 'The automated HEAD probe returned null because the API host root 404s without emitting the header; a real API response does carry "strict-transport-security: max-age=31536000; includeSubDomains; preload". Corrected here from direct observation. The same responses carry X-Content-Type-Options nosniff, X-Frame-Options DENY, Referrer-Policy same-origin and Cross-Origin-Opener-Policy same-origin.'
  observed_on: GET /api/news/ (401 response), 2026-08-11
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: mcp.alphai.io
  hsts: null
  https: true
  note: Header not observed on the 401 challenge; not asserted either way.
  tls_version: TLSv1.3
- host: status.alphai.io
  http_status: 200
  https: true
  note: Status page host, verified reachable 2026-08-11.
kind: domain-security
layout: security
method: probed
name: Alphaai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlphaAI, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AlphaAI
provider_slug: alphaai
slug: alphaai-domain-security
source_filename: alphaai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: >-\n  probe-domain-security.py (DNS/TLS/HTTP HEAD against the apis.yml and OpenAPI\n  servers[] hosts), corrected by direct observation of live API responses on\n  2026-08-11 where the automated HEAD could not read a header.\nhosts:\n  - host: alphai.io\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Oct 19 23:59:59 2026 GMT\n    hsts: false\n    note: >-\n      Next.js behind CloudFront. Serves CSP frame-ancestors 'none' and\n      X-Frame-Options DENY, but no Strict-Transport-Security on the marketing\n      host — the one host most likely to be typed into a browser bar.\n  - host: api.alphai.io\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Feb 10 23:59:59 2027 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: true\n    observed_on: 'GET /api/news/ (401 response), 2026-08-11'\n    note: >-\n      The automated HEAD probe returned null because\
  \ the API host root 404s\n      without emitting the header; a real API response does carry\n      \"strict-transport-security: max-age=31536000; includeSubDomains; preload\".\n      Corrected here from direct observation. The same responses carry\n      X-Content-Type-Options nosniff, X-Frame-Options DENY, Referrer-Policy\n      same-origin and Cross-Origin-Opener-Policy same-origin.\n  - host: mcp.alphai.io\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Feb 10 23:59:59 2027 GMT\n    hsts: null\n    note: Header not observed on the 401 challenge; not asserted either way.\n  - host: status.alphai.io\n    https: true\n    http_status: 200\n    note: Status page host, verified reachable 2026-08-11.\n\ndomains:\n  - domain: alphai.io\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 include:zohomail.com ~all'\n    dmarc: false\n    dmarc_policy: null\n\nfindings:\n  - >-\n    No DMARC record. With SPF set to a soft-fail (~all) and no DMARC policy, the\n\
  \    domain has no enforced anti-spoofing posture — and this provider sends\n    transactional email (alert digests, per-article alerts, webhook auto-disable\n    notices) from it. This is the most actionable item on the list.\n  - No CAA record, so any public CA may issue for the domain.\n  - DNSSEC is not enabled.\n  - >-\n    HSTS is present on the API host with a preload-eligible policy but absent on\n    the website host — the inverse of the usual pattern, and worth flagging\n    because the website is where the account dashboard and API-key issuance live.\n\nother_observations:\n  domain_verifications:\n    - postman-domain-verification (TXT) — corroborates the public Postman workspace\n    - smithery-verification (TXT) — a Smithery MCP registry claim; no live Smithery listing was found for this server on 2026-08-11\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/security/alphaai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Financial News
- Stock Market
- SEC Filings
- Insider Trading
- Fintech
- Market Data
- Sentiment
- AI Agents
- MCP
- LLM
- Trading
---
