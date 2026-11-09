---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: docbin.app
  spf: false
hosts:
- cert_expires: Jan  2 14:46:33 2027 GMT
  host: docbin.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docbin App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for docbin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: docbin
provider_slug: docbin-app
slug: docbin-app-domain-security
source_filename: docbin-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docbin.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 14:46:33 2027 GMT\n  hsts: false\ndomains:\n- domain: docbin.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/docbin-app/security/docbin-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Pastebin
- Markdown
- CLI
- Documentation
---
