---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: albumora.de
  spf: true
hosts:
- host: albumora.de
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Albumora De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for albumora-de, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: albumora-de
provider_slug: albumora-de
slug: albumora-de-domain-security
source_filename: albumora-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: albumora.de\n  https: false\ndomains:\n- domain: albumora.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/albumora-de/security/albumora-de-domain-security.yml
summary_line: DMARC
tags:
- Company
---
