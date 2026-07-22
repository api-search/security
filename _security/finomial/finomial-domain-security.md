---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finomial.com
  spf: true
hosts:
- host: finomial.com
  https: false
kind: domain-security
layout: security
method: probed
name: Finomial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finomial, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Finomial
provider_slug: finomial
slug: finomial-domain-security
source_filename: finomial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finomial.com\n  https: false\ndomains:\n- domain: finomial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finomial/refs/heads/main/security/finomial-domain-security.yml
summary_line: DMARC
tags:
- Company
---
