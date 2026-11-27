---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: attester.dev
  spf: true
hosts:
- host: attester.dev
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: attester-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for attester-dev, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: attester-dev
provider_slug: attester-dev
slug: attester-dev-domain-security
source_filename: attester-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attester.dev\n  https: false\ndomains:\n- domain: attester.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/attester-dev/security/attester-dev-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
