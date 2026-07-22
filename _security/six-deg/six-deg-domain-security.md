---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yellowdig.co
  spf: false
hosts:
- cert_expires: Oct  6 19:55:33 2026 GMT
  host: yellowdig.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Six Deg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Six Deg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Six Deg
provider_slug: six-deg
slug: six-deg-domain-security
source_filename: six-deg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yellowdig.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:55:33 2026 GMT\n  hsts: false\ndomains:\n- domain: yellowdig.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/six-deg/refs/heads/main/security/six-deg-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
