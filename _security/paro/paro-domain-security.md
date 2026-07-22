---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paro.ai
  spf: true
hosts:
- cert_expires: Sep 12 02:14:14 2026 GMT
  host: paro.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Paro
provider_slug: paro
slug: paro-domain-security
source_filename: paro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:14:14 2026 GMT\n  hsts: false\ndomains:\n- domain: paro.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paro/refs/heads/main/security/paro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Accounting
- Marketplace
- Talent
- Fractional CFO
- Bookkeeping
- Professional Services
- AI
---
