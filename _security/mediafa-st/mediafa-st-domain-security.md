---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mediafa.st
  spf: true
hosts:
- cert_expires: Feb 11 17:31:15 2027 GMT
  host: mediafa.st
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MediaFast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediaFast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MediaFast
provider_slug: mediafa-st
slug: mediafa-st-domain-security
source_filename: mediafa-st-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mediafa.st\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 17:31:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mediafa.st\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mediafa-st/security/mediafa-st-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Reddit
- Marketing
- Software-as-a-Service
- Community
- Automation
---
