---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oblixsecurity.com
  spf: true
hosts:
- host: oblixsecurity.com
  https: false
kind: domain-security
layout: security
method: probed
name: Oblix Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oblix Inc., probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oblix Inc.
provider_slug: oblix-inc
slug: oblix-inc-domain-security
source_filename: oblix-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oblixsecurity.com\n  https: false\ndomains:\n- domain: oblixsecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oblix-inc/refs/heads/main/security/oblix-inc-domain-security.yml
summary_line: DMARC
tags:
- Company
---
