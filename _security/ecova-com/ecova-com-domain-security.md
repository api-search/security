---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecova.com
  spf: true
hosts:
- host: www.ecova.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ecova Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ENGIE Insight Services, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ENGIE Insight Services
provider_slug: ecova-com
slug: ecova-com-domain-security
source_filename: ecova-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecova.com\n  https: false\ndomains:\n- domain: ecova.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ecova-com/security/ecova-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
