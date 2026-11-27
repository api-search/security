---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: verirouteintel.com
  spf: true
hosts:
- host: verirouteintel.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: verirouteintel-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for verirouteintel-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: verirouteintel-com
provider_slug: verirouteintel-com
slug: verirouteintel-com-domain-security
source_filename: verirouteintel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verirouteintel.com\n  https: false\ndomains:\n- domain: verirouteintel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/verirouteintel-com/security/verirouteintel-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
