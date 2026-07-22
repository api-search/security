---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: braintripping.com
  spf: true
hosts:
- cert_expires: Sep 18 10:12:02 2026 GMT
  host: www.braintripping.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braintripping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrainTripping, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BrainTripping
provider_slug: braintripping
slug: braintripping-domain-security
source_filename: braintripping-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.braintripping.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:12:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: braintripping.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintripping/refs/heads/main/security/braintripping-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Language
- Games
- Natural Language Processing
- ClojureScript
- Open Source
- Y Combinator
---
