---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: murphy-usa.com
  spf: false
hosts:
- host: www.murphy-usa.com
  https: false
kind: domain-security
layout: security
method: probed
name: Murphy Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for murphy-usa, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: murphy-usa
provider_slug: murphy-usa
slug: murphy-usa-domain-security
source_filename: murphy-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.murphy-usa.com\n  https: false\ndomains:\n- domain: murphy-usa.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/murphy-usa/refs/heads/main/security/murphy-usa-domain-security.yml
summary_line: DMARC
tags:
- Fortune 500
---
