---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: readyforzero.com
  spf: true
hosts:
- host: readyforzero.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Readyforzero Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limbo Labs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Limbo Labs
provider_slug: readyforzero-com
slug: readyforzero-com-domain-security
source_filename: readyforzero-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readyforzero.com\n  https: false\ndomains:\n- domain: readyforzero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/readyforzero-com/security/readyforzero-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
