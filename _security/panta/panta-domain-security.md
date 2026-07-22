---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pantainsure.com
  spf: true
hosts:
- cert_expires: Sep 26 11:11:16 2026 GMT
  host: pantainsure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Panta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Panta
provider_slug: panta
slug: panta-domain-security
source_filename: panta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pantainsure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:11:16 2026 GMT\n  hsts: false\ndomains:\n- domain: pantainsure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panta/refs/heads/main/security/panta-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Insurtech
- Commercial Insurance
- Brokerage
- AI Agents
- Risk Placement
- Excess and Surplus
---
