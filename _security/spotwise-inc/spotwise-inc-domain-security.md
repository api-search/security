---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spotwise.ai
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: spotwise.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: app.spotwise.ai
  hsts: false
  hsts_correction:
    header: 'strict-transport-security: max-age=31536000; includeSubDomains'
    note: 'The automated probe reads GET https://app.spotwise.ai/, which is a bare 307 redirect to /auth/sign-in carrying no headers, so it records hsts:false. Every real application response from this host DOES send HSTS with a one-year max-age and includeSubDomains, verified on GET /docs and POST /api/mcp on 2026-08-12, alongside x-frame-options: DENY, x-content-type-options: nosniff, referrer-policy: strict-origin-when-cross-origin, cross-origin-opener-policy and cross-origin-resource-policy: same-origin. Read hsts:false on this host as a probe artefact, not a finding.'
    observed: true
  hsts_effective: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spotwise Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spotwise, Inc., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spotwise, Inc.
provider_slug: spotwise-inc
slug: spotwise-inc-domain-security
source_filename: spotwise-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spotwise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: app.spotwise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\n  hsts_correction:\n    observed: true\n    header: 'strict-transport-security: max-age=31536000; includeSubDomains'\n    note: >-\n      The automated probe reads GET https://app.spotwise.ai/, which is a bare 307\n      redirect to /auth/sign-in carrying no headers, so it records hsts:false. Every\n      real application response from this host DOES send HSTS with a one-year max-age\n      and includeSubDomains, verified on GET /docs and POST /api/mcp on 2026-08-12,\n      alongside x-frame-options: DENY, x-content-type-options: nosniff,\n      referrer-policy: strict-origin-when-cross-origin, cross-origin-opener-policy and\n    \
  \  cross-origin-resource-policy: same-origin. Read hsts:false on this host as a\n      probe artefact, not a finding.\n  hsts_effective: true\ndomains:\n- domain: spotwise.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotwise-inc/refs/heads/main/security/spotwise-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Broadcast Media
- Advertising
- Media Monitoring
- Sales Intelligence
- Lead Generation
- Artificial Intelligence
- Radio
- MCP
- Agents
- Attribution
---
