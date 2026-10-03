---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boxnutt.com
  spf: false
hosts:
- cert_expires: Dec 24 05:32:15 2026 GMT
  host: boxnutt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boxnutt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boxnutt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Boxnutt
provider_slug: boxnutt
slug: boxnutt-domain-security
source_filename: boxnutt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boxnutt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 05:32:15 2026 GMT\n  hsts: false\ndomains:\n- domain: boxnutt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boxnutt/refs/heads/main/security/boxnutt-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Adult
- Media
- Blog
- Content
---
