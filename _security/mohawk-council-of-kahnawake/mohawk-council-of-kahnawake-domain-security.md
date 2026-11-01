---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kahnawake.com
  spf: true
hosts:
- host: www.kahnawake.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mohawk Council Of Kahnawake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mohawk Council of Kahnawake, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mohawk Council of Kahnawake
provider_slug: mohawk-council-of-kahnawake
slug: mohawk-council-of-kahnawake-domain-security
source_filename: mohawk-council-of-kahnawake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kahnawake.com\n  https: false\ndomains:\n- domain: kahnawake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mohawk-council-of-kahnawake/security/mohawk-council-of-kahnawake-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Community Services
- Social Assistance
- Land Management
- Housing
- Finance
- Public Safety
---
