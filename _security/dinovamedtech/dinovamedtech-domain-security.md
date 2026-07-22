---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: dinovamedtech.com
  mx: []
  nameservers:
  - amanda.ns.cloudflare.com
  - ken.ns.cloudflare.com
  spf: false
hosts:
- host: dinovamedtech.com
  hsts: false
  hsts_max_age: null
  https: false
  reachable: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Dinovamedtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dinovamedtech, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: dinovamedtech
provider_slug: dinovamedtech
slug: dinovamedtech-domain-security
source_filename: dinovamedtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: dig + TLS/HTTP HEAD on dinovamedtech.com\nnotes: >-\n  Domain resolves (A 156.237.181.215) and delegates to Cloudflare nameservers,\n  but the web server did not respond on HTTPS or HTTP (connection timed out /\n  refused during this probe). No email or domain-hardening DNS records are\n  published. Absence of records is valid recorded data, not a fabrication.\nhosts:\n  - host: dinovamedtech.com\n    https: false\n    reachable: false\n    tls_version: null\n    hsts: false\n    hsts_max_age: null\ndomains:\n  - domain: dinovamedtech.com\n    nameservers: [amanda.ns.cloudflare.com, ken.ns.cloudflare.com]\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinovamedtech/refs/heads/main/security/dinovamedtech-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
