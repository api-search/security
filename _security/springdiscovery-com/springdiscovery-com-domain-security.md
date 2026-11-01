---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: springdiscovery.com
  spf: true
hosts:
- host: www.springdiscovery.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Springdiscovery Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spring
provider_slug: springdiscovery-com
slug: springdiscovery-com-domain-security
source_filename: springdiscovery-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.springdiscovery.com\n  https: false\ndomains:\n- domain: springdiscovery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/springdiscovery-com/security/springdiscovery-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
