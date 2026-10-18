---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jedlix.com
  spf: true
hosts:
- host: www.jedlix.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jedlix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jedlix, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jedlix
provider_slug: jedlix
slug: jedlix-domain-security
source_filename: jedlix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jedlix.com\n  https: false\ndomains:\n- domain: jedlix.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jedlix/refs/heads/main/security/jedlix-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Fintech
- Electric Vehicles
- Charging
- Energy
---
