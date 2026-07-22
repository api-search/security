---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: accion-systems.com
  spf: true
hosts:
- host: www.accion-systems.com
  https: false
kind: domain-security
layout: security
method: probed
name: Accion Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accion Systems, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Accion Systems
provider_slug: accion-systems
slug: accion-systems-domain-security
source_filename: accion-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accion-systems.com\n  https: false\ndomains:\n- domain: accion-systems.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accion-systems/refs/heads/main/security/accion-systems-domain-security.yml
summary_line: DMARC
tags:
- Company
- Aerospace
---
