---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashquark.io
  spf: true
hosts:
- host: hashquark.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hashquark Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hashquark, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: hashquark
provider_slug: hashquark-io
slug: hashquark-io-domain-security
source_filename: hashquark-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hashquark.io\n  https: false\ndomains:\n- domain: hashquark.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hashquark-io/security/hashquark-io-domain-security.yml
summary_line: DMARC
tags:
- Company
- Blockchain
- Cryptocurrency
- APIs
- DeveloperTools
---
