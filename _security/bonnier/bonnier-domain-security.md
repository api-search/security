---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bonnier.com
  spf: true
hosts:
- host: bonnier.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bonnier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonnier, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bonnier
provider_slug: bonnier
slug: bonnier-domain-security
source_filename: bonnier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bonnier.com\n  https: false\ndomains:\n- domain: bonnier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonnier/refs/heads/main/security/bonnier-domain-security.yml
summary_line: DMARC
tags:
- Company
---
