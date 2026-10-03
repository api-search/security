---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: proteusmotion.com
  spf: true
hosts:
- cert_expires: Nov 12 06:45:20 2026 GMT
  host: proteusmotion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bostonbiomotion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bostonbiomotion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bostonbiomotion
provider_slug: bostonbiomotion
slug: bostonbiomotion-domain-security
source_filename: bostonbiomotion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proteusmotion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 06:45:20 2026 GMT\n  hsts: false\ndomains:\n- domain: proteusmotion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bostonbiomotion/refs/heads/main/security/bostonbiomotion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
