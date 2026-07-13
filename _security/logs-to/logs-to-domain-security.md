---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: logs.to
  spf: false
hosts:
- cert_expires: Aug 19 19:24:25 2026 GMT
  host: logs.to
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logs To Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logs.to, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Logs.to
provider_slug: logs-to
slug: logs-to-domain-security
source_filename: logs-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logs.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:24:25 2026 GMT\n  hsts: false\ndomains:\n- domain: logs.to\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logs-to/refs/heads/main/security/logs-to-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
