---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: promptable.ai
  spf: true
hosts:
- cert_expires: Apr  1 10:32:39 2027 GMT
  host: promptable.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Promptable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Promptable
provider_slug: promptable
slug: promptable-domain-security
source_filename: promptable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 10:32:39 2027 GMT\n  hsts: false\ndomains:\n- domain: promptable.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/promptable/security/promptable-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
