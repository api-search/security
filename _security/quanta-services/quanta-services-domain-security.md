---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quanta-services.com
  spf: true
hosts:
- host: www.quanta-services.com
  https: false
kind: domain-security
layout: security
method: probed
name: Quanta Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quanta Services, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quanta Services
provider_slug: quanta-services
slug: quanta-services-domain-security
source_filename: quanta-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quanta-services.com\n  https: false\ndomains:\n- domain: quanta-services.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quanta-services/refs/heads/main/security/quanta-services-domain-security.yml
summary_line: DMARC
tags:
- Fortune 500
- Infrastructure
- Energy
- Electric Power
- Renewable Energy
- Pipeline
- Communications
---
