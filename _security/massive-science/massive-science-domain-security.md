---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: massivesci.com
  spf: false
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: massivesci.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Massive Science Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Massive Science, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Massive Science
provider_slug: massive-science
slug: massive-science-domain-security
source_filename: massive-science-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: massivesci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: massivesci.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/massive-science/refs/heads/main/security/massive-science-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Science
- Media
- Publishing
- Science Communication
- Journalism
- Content
---
