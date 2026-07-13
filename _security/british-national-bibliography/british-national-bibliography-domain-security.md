---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bl.uk
  spf: true
hosts:
- host: bnb.data.bl.uk
  https: false
kind: domain-security
layout: security
method: probed
name: British National Bibliography Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for British National Bibliography, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: British National Bibliography
provider_slug: british-national-bibliography
slug: british-national-bibliography-domain-security
source_filename: british-national-bibliography-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bnb.data.bl.uk\n  https: false\ndomains:\n- domain: bl.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/british-national-bibliography/refs/heads/main/security/british-national-bibliography-domain-security.yml
summary_line: DMARC
tags:
- Books
- Public APIs
---
