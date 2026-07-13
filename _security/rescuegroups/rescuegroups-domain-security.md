---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rescuegroups.org
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: userguide.rescuegroups.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rescuegroups Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RescueGroups, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RescueGroups
provider_slug: rescuegroups
slug: rescuegroups-domain-security
source_filename: rescuegroups-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userguide.rescuegroups.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: rescuegroups.org\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rescuegroups/refs/heads/main/security/rescuegroups-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animals
- Public APIs
---
