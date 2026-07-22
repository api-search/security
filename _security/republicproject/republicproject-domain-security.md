---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: republicproject.com
  spf: false
hosts:
- host: republicproject.com
  https: false
kind: domain-security
layout: security
method: probed
name: Republicproject Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RepublicProject, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: RepublicProject
provider_slug: republicproject
slug: republicproject-domain-security
source_filename: republicproject-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: republicproject.com\n  https: false\ndomains:\n- domain: republicproject.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/republicproject/refs/heads/main/security/republicproject-domain-security.yml
summary_line: DMARC
tags:
- Company
---
