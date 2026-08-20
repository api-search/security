---
api_specs:
- filename: datarails-financeos-mcp-openapi.json
  format: json
  label: Datarails FinanceOS MCP Server
  slug: financeos-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/openapi/datarails-financeos-mcp-openapi.json
description: Transport and DNS security posture, probed directly. The application and API hosts are consistently strong (TLS 1.3, HSTS at 180 days); the marketing host ships no HSTS header at all, and the registrable domain has neither DNSSEC nor a CAA record. Email authentication is the strongest part of the posture — SPF with a hard fail and DMARC at p=reject.
domains:
- caa: []
  caa_evidence: no CAA records returned — any public CA may issue for this domain
  dmarc: true
  dmarc_aggregate_reporting: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:dmarc@datarails.com, mailto:rpy61q5g9y@rua.powerdmarc.com
  dnssec: false
  dnssec_evidence: no DNSKEY records returned
  domain: datarails.com
  spf: true
  spf_policy: hard fail (-all)
  spf_record: v=spf1 include:mail.zendesk.com mx include:_spf.google.com include:6909491.spf10.hubspotemail.net include:amazonses.com -all
hosts:
- cdn: Cloudflare
  cert_issuer: Google Trust Services (WE1)
  cert_not_after: '2026-10-14'
  host: mcp.datarails.com
  hsts: true
  hsts_includesubdomains: false
  hsts_max_age: 15552000
  hsts_preload: false
  https: true
  role: FinanceOS MCP server
  security_headers:
    permissions-policy: present (geolocation, microphone, camera, gyroscope, magnetometer, payment, usb, midi, push all disabled)
    referrer-policy: strict-origin-when-cross-origin
    x-content-type-options: nosniff
    x-permitted-cross-domain-policies: none
  tls_version: TLSv1.3
- cert_issuer: Google Trust Services (WE1)
  cert_not_after: '2026-10-14'
  host: app.datarails.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: Redirects to https://auth.datarails.com/ when unauthenticated.
  role: Datarails application and Data Gateway Service REST endpoint
  tls_version: TLSv1.3
- cert_issuer: Google Trust Services (WE1)
  cert_not_after: '2026-10-14'
  host: auth.datarails.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  role: Authentication / SSO entry point
  tls_version: TLSv1.3
- cert_issuer: Let's Encrypt (YE2)
  cert_not_after: '2026-09-26'
  host: www.datarails.com
  hsts: false
  hsts_max_age: null
  https: true
  note: No Strict-Transport-Security header on the marketing host. Also returns HTTP 403 to non-browser user agents (bot protection), which is why the site pages were read through a browser-class fetch.
  role: Marketing site and llms.txt
  tls_version: TLSv1.3
- host: trust.datarails.com
  https: true
  note: Third-party hosted; not probed for TLS parameters.
  role: Trust center (Vendict-hosted)
- host: support.datarails.com
  https: true
  note: Third-party hosted; returns 403 to non-browser user agents.
  role: Help center (Zendesk-hosted)
kind: domain-security
layout: security
method: probed
name: Datarails Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datarails, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datarails
provider_slug: datarails
slug: datarails-domain-security
source_filename: datarails-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS and TLS probe of every Datarails host in apis.yml\ndescription: >-\n  Transport and DNS security posture, probed directly. The application and API\n  hosts are consistently strong (TLS 1.3, HSTS at 180 days); the marketing host\n  ships no HSTS header at all, and the registrable domain has neither DNSSEC\n  nor a CAA record. Email authentication is the strongest part of the posture —\n  SPF with a hard fail and DMARC at p=reject.\n\nhosts:\n  - host: mcp.datarails.com\n    role: FinanceOS MCP server\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: Google Trust Services (WE1)\n    cert_not_after: '2026-10-14'\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_includesubdomains: false\n    hsts_preload: false\n    security_headers:\n      x-content-type-options: nosniff\n      referrer-policy: strict-origin-when-cross-origin\n      x-permitted-cross-domain-policies: none\n      permissions-policy: present\
  \ (geolocation, microphone, camera, gyroscope, magnetometer, payment, usb, midi, push all disabled)\n    cdn: Cloudflare\n  - host: app.datarails.com\n    role: Datarails application and Data Gateway Service REST endpoint\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: Google Trust Services (WE1)\n    cert_not_after: '2026-10-14'\n    hsts: true\n    hsts_max_age: 15552000\n    note: Redirects to https://auth.datarails.com/ when unauthenticated.\n  - host: auth.datarails.com\n    role: Authentication / SSO entry point\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: Google Trust Services (WE1)\n    cert_not_after: '2026-10-14'\n    hsts: true\n    hsts_max_age: 15552000\n  - host: www.datarails.com\n    role: Marketing site and llms.txt\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: Let's Encrypt (YE2)\n    cert_not_after: '2026-09-26'\n    hsts: false\n    hsts_max_age: null\n    note: >-\n      No Strict-Transport-Security header on the marketing\
  \ host. Also returns\n      HTTP 403 to non-browser user agents (bot protection), which is why the\n      site pages were read through a browser-class fetch.\n  - host: trust.datarails.com\n    role: Trust center (Vendict-hosted)\n    https: true\n    note: Third-party hosted; not probed for TLS parameters.\n  - host: support.datarails.com\n    role: Help center (Zendesk-hosted)\n    https: true\n    note: Third-party hosted; returns 403 to non-browser user agents.\n\ndomains:\n  - domain: datarails.com\n    dnssec: false\n    dnssec_evidence: no DNSKEY records returned\n    caa: []\n    caa_evidence: no CAA records returned — any public CA may issue for this domain\n    spf: true\n    spf_record: 'v=spf1 include:mail.zendesk.com mx include:_spf.google.com include:6909491.spf10.hubspotemail.net include:amazonses.com -all'\n    spf_policy: hard fail (-all)\n    dmarc: true\n    dmarc_policy: reject\n    dmarc_record: 'v=DMARC1; p=reject; rua=mailto:dmarc@datarails.com, mailto:rpy61q5g9y@rua.powerdmarc.com'\n\
  \    dmarc_aggregate_reporting: true\n\nthird_party_domain_verifications:\n  note: >-\n    TXT records on datarails.com show which platforms Datarails has verified\n    domain ownership with. Recorded because it corroborates the AI-connector\n    surface.\n  records:\n    - google-site-verification\n    - openai-domain-verification\n    - lovable_verification\n    - mongodb-site-verification\n    - 'MS= (Microsoft)'\n\nfindings:\n  - severity: medium\n    finding: No CAA record on datarails.com — certificate issuance is not restricted to named CAs.\n  - severity: medium\n    finding: No DNSSEC on datarails.com.\n  - severity: low\n    finding: No HSTS on www.datarails.com; the application, auth and API hosts all carry it at 180 days.\n  - severity: info\n    finding: No HSTS preload and no includeSubDomains on any host.\n  - severity: positive\n    finding: DMARC at p=reject with aggregate reporting, and SPF with a hard fail.\n  - severity: positive\n    finding: TLS 1.3 on every first-party\
  \ host, with a full modern security-header set on the MCP host.\n\nx-evidence:\n  fetched: '2026-08-01'\n  tools: [dig, 'openssl s_client', 'curl -D']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/security/datarails-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Accounting
- Budgeting
- Forecasting
- Business Intelligence
- Reporting
- Data Integration
- MCP
- Artificial Intelligence
- Excel
- Software-as-a-Service
---
