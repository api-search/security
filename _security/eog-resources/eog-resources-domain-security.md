---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: eog-resources.com
  spf: false
hosts:
- host: www.eog-resources.com
  https: false
kind: domain-security
layout: security
method: probed
name: Eog Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eog-resources, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: eog-resources
provider_slug: eog-resources
slug: eog-resources-domain-security
source_filename: eog-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eog-resources.com\n  https: false\ndomains:\n- domain: eog-resources.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eog-resources/refs/heads/main/security/eog-resources-domain-security.yml
summary_line: DNSSEC
tags:
- Fortune 500
---
