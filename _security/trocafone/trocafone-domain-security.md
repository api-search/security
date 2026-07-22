---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: true
  domain: trocafone.com.br
  spf: false
hosts:
- host: trocafone.com.br
  https: false
kind: domain-security
layout: security
method: probed
name: Trocafone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trocafone, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Trocafone
provider_slug: trocafone
slug: trocafone-domain-security
source_filename: trocafone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trocafone.com.br\n  https: false\ndomains:\n- domain: trocafone.com.br\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trocafone/refs/heads/main/security/trocafone-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- E-Commerce
- Refurbished Electronics
- Marketplace
- Mobile Devices
- Trade-In
- Consumer Electronics
- Brazil
---
