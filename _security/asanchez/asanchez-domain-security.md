---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: asanchez.dev
  spf: true
hosts:
- cert_expires: Dec 27 08:23:11 2026 GMT
  host: asanchez.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asanchez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Prompto
provider_slug: asanchez
slug: asanchez-domain-security
source_filename: asanchez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asanchez.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 08:23:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: asanchez.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asanchez/refs/heads/main/security/asanchez-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
---
