---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: srv.us
  spf: false
hosts:
- cert_expires: Jan  4 11:14:17 2027 GMT
  host: srv.us
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Srv Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for srv-us, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: srv-us
provider_slug: srv-us
slug: srv-us-domain-security
source_filename: srv-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: srv.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 11:14:17 2027 GMT\n  hsts: false\ndomains:\n- domain: srv.us\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/srv-us/security/srv-us-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Platform
- TLS
- SSH
- DeveloperTools
- OpenSource
- Company
---
