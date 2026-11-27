---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mascowiz.com
  spf: true
hosts:
- cert_expires: Dec 18 12:33:31 2026 GMT
  host: mascowiz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mascowiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mascowiz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mascowiz
provider_slug: mascowiz-com
slug: mascowiz-com-domain-security
source_filename: mascowiz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mascowiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mascowiz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mascowiz-com/security/mascowiz-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Animation
- Mascot
- MCP
---
