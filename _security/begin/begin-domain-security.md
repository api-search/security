---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: begin.com
  spf: false
hosts:
- cert_expires: Jan 19 21:39:19 2027 GMT
  host: www.begin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Begin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Begin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Begin
provider_slug: begin
slug: begin-domain-security
source_filename: begin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.begin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 21:39:19 2027 GMT\n  hsts: null\ndomains:\n- domain: begin.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/begin/security/begin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- DeveloperTools
- Platform
- Startup
---
