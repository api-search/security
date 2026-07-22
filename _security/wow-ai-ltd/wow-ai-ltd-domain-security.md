---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getwow.ai
  spf: true
hosts:
- cert_expires: Sep 23 12:08:49 2026 GMT
  host: getwow.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wow Ai Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wow AI LTD., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wow AI LTD.
provider_slug: wow-ai-ltd
slug: wow-ai-ltd-domain-security
source_filename: wow-ai-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getwow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:08:49 2026 GMT\n  hsts: false\ndomains:\n- domain: getwow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wow-ai-ltd/refs/heads/main/security/wow-ai-ltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
