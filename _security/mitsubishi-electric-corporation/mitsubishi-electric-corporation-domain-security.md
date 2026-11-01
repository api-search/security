---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mitsubishielectric.com
  spf: true
hosts:
- host: global.mitsubishielectric.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mitsubishi Electric Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitsubishi Electric Corporation, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mitsubishi Electric Corporation
provider_slug: mitsubishi-electric-corporation
slug: mitsubishi-electric-corporation-domain-security
source_filename: mitsubishi-electric-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.mitsubishielectric.com\n  https: false\ndomains:\n- domain: mitsubishielectric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mitsubishi-electric-corporation/security/mitsubishi-electric-corporation-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
