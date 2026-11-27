---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jvn.jp
  spf: true
hosts:
- cert_expires: Jan 31 14:59:00 2027 GMT
  host: jvn.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JVN (Japan Vulnerability Notes) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JVN (Japan Vulnerability Notes), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: JVN (Japan Vulnerability Notes)
provider_slug: jvn
slug: jvn-domain-security
source_filename: jvn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jvn.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 14:59:00 2027 GMT\n  hsts: false\ndomains:\n- domain: jvn.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jvn/security/jvn-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Security
- Vulnerabilities
- Japan
- Government
---
