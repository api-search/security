---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unplu.gg
  spf: false
hosts:
- cert_expires: Aug 31 21:06:40 2026 GMT
  host: unplu.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unplugg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unplugg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Unplugg
provider_slug: unplugg
slug: unplugg-domain-security
source_filename: unplugg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unplu.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:06:40 2026 GMT\n  hsts: false\ndomains:\n- domain: unplu.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unplugg/refs/heads/main/security/unplugg-domain-security.yml
summary_line: TLSv1.3
tags:
- Machine Learning
- Public APIs
---
