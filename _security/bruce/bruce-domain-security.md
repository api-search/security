---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bruce.bot
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: bruce.bot
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bruce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bruce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bruce
provider_slug: bruce
slug: bruce-domain-security
source_filename: bruce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bruce.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bruce.bot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bruce/refs/heads/main/security/bruce-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplaces
- Real Estate
- Mortgage
- Insurance
- Title and Escrow
- Reputation
- Professional Network
- Artificial Intelligence
---
