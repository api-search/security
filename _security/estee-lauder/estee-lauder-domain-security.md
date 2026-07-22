---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: estee-lauder.com
  spf: false
hosts:
- host: www.estee-lauder.com
  https: false
kind: domain-security
layout: security
method: probed
name: Estee Lauder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for estee-lauder, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: estee-lauder
provider_slug: estee-lauder
slug: estee-lauder-domain-security
source_filename: estee-lauder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.estee-lauder.com\n  https: false\ndomains:\n- domain: estee-lauder.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estee-lauder/refs/heads/main/security/estee-lauder-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Fortune 500
---
