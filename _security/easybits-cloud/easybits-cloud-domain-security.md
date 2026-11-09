---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easybits.cloud
  spf: true
hosts:
- host: easybits.cloud
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easybits Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for easybits-cloud, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: easybits-cloud
provider_slug: easybits-cloud
slug: easybits-cloud-domain-security
source_filename: easybits-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easybits.cloud\n  https: false\ndomains:\n- domain: easybits.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easybits-cloud/security/easybits-cloud-domain-security.yml
summary_line: DMARC
tags:
- Company
---
