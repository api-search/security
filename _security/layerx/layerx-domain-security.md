---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: layerx.co.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bakuraku.jp
  spf: false
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: layerx.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: bakuraku.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.bakuraku.layerx.jp
  hsts: true
  hsts_header: max-age=15552000; includeSubDomains
  hsts_note: 'The probe read the host root, which the ALB answers with a bare empty 404 carrying no headers. A manual anonymous GET of https://api.bakuraku.layerx.jp/rest/v1/tenant/users on 2026-08-23 returned strict-transport-security: max-age=15552000; includeSubDomains alongside x-content-type-options: nosniff, x-frame-options: SAMEORIGIN and x-permitted-cross-domain-policies: none. HSTS is present on the API path, absent from the ALB''s catch-all 404.'
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Layerx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LayerX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LayerX
provider_slug: layerx
slug: layerx-domain-security
source_filename: layerx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layerx.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\n- host: bakuraku.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.bakuraku.layerx.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_header: 'max-age=15552000; includeSubDomains'\n  hsts_note: >-\n    The probe read the host root, which the ALB answers with a bare empty 404 carrying no\n    headers. A manual anonymous GET of https://api.bakuraku.layerx.jp/rest/v1/tenant/users\n    on 2026-08-23 returned strict-transport-security: max-age=15552000; includeSubDomains\n    alongside x-content-type-options: nosniff, x-frame-options: SAMEORIGIN and\n    x-permitted-cross-domain-policies: none. HSTS is present on the API path, absent from\n\
  \    the ALB's catch-all 404.\ndomains:\n- domain: layerx.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bakuraku.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\nnotes:\n- >-\n    Neither layerx.co.jp nor bakuraku.jp publishes a CAA record or signs its zone with\n    DNSSEC. bakuraku.jp has no SPF record; layerx.co.jp does. Both DMARC policies are\n    p=none, i.e. monitoring only — nothing is quarantined or rejected on a failure.\n- >-\n    api.bakuraku.layerx.jp negotiates TLS 1.2 while the two web hosts negotiate TLS 1.3;\n    Bakuraku's own security page claims TLS 1.3 for communications, which holds for the\n    product hosts but not for the API host as probed on 2026-08-23.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layerx/refs/heads/main/security/layerx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Japan
- Back Office
- Expense Management
- Invoicing
- Accounts Payable
- Workflow
- Approvals
- Accounting
- Payroll
- Attendance
- Corporate Cards
- Artificial Intelligence
- AI Agents
- Document Processing
- SaaS
- Enterprise Software
- Fintech
---
