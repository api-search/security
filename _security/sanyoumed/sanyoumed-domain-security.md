---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sanyoumed.com
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: sanyoumed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sanyoumed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sanyoumed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: sanyoumed
provider_slug: sanyoumed
slug: sanyoumed-domain-security
source_filename: sanyoumed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sanyoumed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sanyoumed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanyoumed/refs/heads/main/security/sanyoumed-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
