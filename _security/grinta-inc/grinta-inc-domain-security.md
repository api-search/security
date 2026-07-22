---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: grinta.ai
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: grinta.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grinta Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grinta Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grinta Inc
provider_slug: grinta-inc
slug: grinta-inc-domain-security
source_filename: grinta-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grinta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: grinta.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grinta-inc/refs/heads/main/security/grinta-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
