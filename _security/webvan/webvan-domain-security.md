---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webvan.com
  spf: true
hosts:
- host: www.webvan.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Webvan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webvan, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Webvan
provider_slug: webvan
slug: webvan-domain-security
source_filename: webvan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.webvan.com\n  https: false\ndomains:\n- domain: webvan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webvan/refs/heads/main/security/webvan-domain-security.yml
summary_line: DMARC
tags:
- Company
- Grocery
- Delivery
- E-Commerce
- Startups
- Technology
---
