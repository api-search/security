---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elsas.it
  spf: true
hosts:
- host: elsas.it
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: elsas-it Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for elsas-it, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: elsas-it
provider_slug: elsas-it
slug: elsas-it-domain-security
source_filename: elsas-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elsas.it\n  https: false\ndomains:\n- domain: elsas.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/elsas-it/security/elsas-it-domain-security.yml
summary_line: DMARC
tags:
- Company
---
