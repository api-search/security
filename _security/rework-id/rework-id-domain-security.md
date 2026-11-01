---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: rework.id
  spf: true
hosts:
- host: rework.id
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rework Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoWork, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GoWork
provider_slug: rework-id
slug: rework-id-domain-security
source_filename: rework-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rework.id\n  https: false\ndomains:\n- domain: rework.id\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rework-id/security/rework-id-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
