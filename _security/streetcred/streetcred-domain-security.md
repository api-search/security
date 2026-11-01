---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: streetcred.co
  spf: true
hosts:
- host: www.streetcred.co
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Streetcred Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StreetCred, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StreetCred
provider_slug: streetcred
slug: streetcred-domain-security
source_filename: streetcred-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.streetcred.co\n  https: false\ndomains:\n- domain: streetcred.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/streetcred/security/streetcred-domain-security.yml
summary_line: DMARC
tags:
- Company
---
