---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: brainscanner.dev
  spf: true
hosts:
- cert_expires: Jan  8 17:11:35 2027 GMT
  host: brainscanner.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainscanner Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brain Scanner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Brain Scanner
provider_slug: brainscanner-dev
slug: brainscanner-dev-domain-security
source_filename: brainscanner-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainscanner.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 17:11:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brainscanner.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/brainscanner-dev/security/brainscanner-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- AI Coding
- Code Review
- Session Replay
- Task Queue
---
