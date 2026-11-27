---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marqpdf.com
  spf: true
hosts:
- host: marqpdf.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: marqpdf-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for marqpdf-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: marqpdf-com
provider_slug: marqpdf-com
slug: marqpdf-com-domain-security
source_filename: marqpdf-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marqpdf.com\n  https: false\ndomains:\n- domain: marqpdf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/marqpdf-com/security/marqpdf-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
