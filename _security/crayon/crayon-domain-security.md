---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crayon.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crayon.com
  spf: true
hosts:
- cert_expires: Sep 21 00:09:20 2026 GMT
  host: www.crayon.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 13:48:02 2026 GMT
  host: apidocs.crayon.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 15 14:39:26 2026 GMT
  host: api.crayon.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Crayon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crayon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crayon
provider_slug: crayon
slug: crayon-domain-security
source_filename: crayon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crayon.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:09:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.crayon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 13:48:02 2026 GMT\n  hsts: false\n- host: api.crayon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 15 14:39:26 2026 GMT\n  hsts: null\ndomains:\n- domain: crayon.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: crayon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/security/crayon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Competitive Intelligence
- Market Intelligence
- Sales Enablement
- Battlecards
- Win-Loss Analysis
- AI
- MCP
---
