---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: verbmax.com
  spf: false
hosts:
- cert_expires: Jan  1 23:02:02 2027 GMT
  host: verbmax.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Verbmax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verbmax AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Verbmax AI
provider_slug: verbmax
slug: verbmax-domain-security
source_filename: verbmax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verbmax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:02:02 2027 GMT\n  hsts: false\ndomains:\n- domain: verbmax.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/verbmax/security/verbmax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
