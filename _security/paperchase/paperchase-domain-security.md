---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paperchase.co.uk
  spf: true
hosts:
- host: paperchase.co.uk
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Paperchase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paperchase, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paperchase
provider_slug: paperchase
slug: paperchase-domain-security
source_filename: paperchase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paperchase.co.uk\n  https: false\ndomains:\n- domain: paperchase.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/paperchase/security/paperchase-domain-security.yml
summary_line: DMARC
tags:
- Company
---
