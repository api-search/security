---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: npr.org
  spf: true
hosts:
- host: dev.npr.org
  https: false
kind: domain-security
layout: security
method: probed
name: Npr One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NPR One, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NPR One
provider_slug: npr-one
slug: npr-one-domain-security
source_filename: npr-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.npr.org\n  https: false\ndomains:\n- domain: npr.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npr-one/refs/heads/main/security/npr-one-domain-security.yml
summary_line: DMARC
tags:
- News
- Public APIs
---
