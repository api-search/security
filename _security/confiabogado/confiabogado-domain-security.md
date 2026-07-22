---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: confiabogado.com
  spf: false
hosts:
- host: confiabogado.com
  https: false
kind: domain-security
layout: security
method: probed
name: Confiabogado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConfiAbogado, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: ConfiAbogado
provider_slug: confiabogado
slug: confiabogado-domain-security
source_filename: confiabogado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: confiabogado.com\n  https: false\ndomains:\n- domain: confiabogado.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confiabogado/refs/heads/main/security/confiabogado-domain-security.yml
summary_line: DMARC
tags:
- Company
---
