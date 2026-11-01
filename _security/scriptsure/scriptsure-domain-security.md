---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scriptsure.com
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: scriptsure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scriptsure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScriptSure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ScriptSure
provider_slug: scriptsure
slug: scriptsure-domain-security
source_filename: scriptsure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scriptsure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: scriptsure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/scriptsure/security/scriptsure-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
