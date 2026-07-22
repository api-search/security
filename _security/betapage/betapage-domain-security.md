---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: betapage.co
  spf: true
hosts:
- cert_expires: Sep  5 13:11:29 2026 GMT
  host: betapage.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betapage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetaPage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BetaPage
provider_slug: betapage
slug: betapage-domain-security
source_filename: betapage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betapage.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:11:29 2026 GMT\n  hsts: false\ndomains:\n- domain: betapage.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betapage/refs/heads/main/security/betapage-domain-security.yml
summary_line: TLSv1.3
tags:
- Startups
- Product Launch
- Startup Directory
- Early Adopters
- Beta Testing
---
