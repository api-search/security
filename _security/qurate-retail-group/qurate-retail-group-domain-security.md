---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qurate-retail-group.com
  spf: true
hosts:
- host: www.qurate-retail-group.com
  https: false
kind: domain-security
layout: security
method: probed
name: Qurate Retail Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qurate Retail Group, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qurate Retail Group
provider_slug: qurate-retail-group
slug: qurate-retail-group-domain-security
source_filename: qurate-retail-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qurate-retail-group.com\n  https: false\ndomains:\n- domain: qurate-retail-group.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qurate-retail-group/refs/heads/main/security/qurate-retail-group-domain-security.yml
summary_line: DMARC
tags:
- Retail
- Ecommerce
- Video Commerce
- Fortune 500
---
