---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 1910genetics.com
  spf: true
hosts:
- host: www.1910genetics.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1910Genetics Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1910 Genetics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 1910 Genetics
provider_slug: 1910genetics-com
slug: 1910genetics-com-domain-security
source_filename: 1910genetics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1910genetics.com\n  https: false\ndomains:\n- domain: 1910genetics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/1910genetics-com/security/1910genetics-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
