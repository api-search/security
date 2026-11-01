---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intesta.io
  spf: false
hosts:
- host: intesta.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intesta Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for intesta-io, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: intesta-io
provider_slug: intesta-io
slug: intesta-io-domain-security
source_filename: intesta-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intesta.io\n  https: false\ndomains:\n- domain: intesta.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/intesta-io/security/intesta-io-domain-security.yml
summary_line: DMARC
tags:
- Company
---
