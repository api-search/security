---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: borderconnect.com
  spf: true
hosts:
- host: borderconnect.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BorderConnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BorderConnect, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BorderConnect
provider_slug: borderconnect
slug: borderconnect-domain-security
source_filename: borderconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: borderconnect.com\n  https: false\ndomains:\n- domain: borderconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/borderconnect/security/borderconnect-domain-security.yml
summary_line: DMARC
tags:
- Company
---
