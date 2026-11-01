---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drobo.com
  spf: true
hosts:
- host: www.drobo.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drobo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drobo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Drobo
provider_slug: drobo
slug: drobo-domain-security
source_filename: drobo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drobo.com\n  https: false\ndomains:\n- domain: drobo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/drobo/security/drobo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Storage
- DataManagement
- SmallBusiness
- Enterprise
---
