---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tradebrite.nl
  spf: true
hosts:
- cert_expires: Dec 15 09:46:40 2026 GMT
  host: tradebrite.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tradebrite Nl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tradebrite-nl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: tradebrite-nl
provider_slug: tradebrite-nl
slug: tradebrite-nl-domain-security
source_filename: tradebrite-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradebrite.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 09:46:40 2026 GMT\n  hsts: false\ndomains:\n- domain: tradebrite.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tradebrite-nl/security/tradebrite-nl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Automation
- Development
- Netherlands
- Services
---
