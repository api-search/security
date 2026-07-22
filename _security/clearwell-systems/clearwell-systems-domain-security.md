---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clearwellsystems.com
  spf: true
hosts:
- host: www.clearwellsystems.com
  https: false
kind: domain-security
layout: security
method: probed
name: Clearwell Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearwell Systems, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Clearwell Systems
provider_slug: clearwell-systems
slug: clearwell-systems-domain-security
source_filename: clearwell-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearwellsystems.com\n  https: false\ndomains:\n- domain: clearwellsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearwell-systems/refs/heads/main/security/clearwell-systems-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
