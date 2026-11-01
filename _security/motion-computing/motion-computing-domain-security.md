---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: true
  domain: motioncomputing.com
  spf: false
hosts:
- host: motioncomputing.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Motion Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motion Computing, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Motion Computing
provider_slug: motion-computing
slug: motion-computing-domain-security
source_filename: motion-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motioncomputing.com\n  https: false\ndomains:\n- domain: motioncomputing.com\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/motion-computing/security/motion-computing-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---
