---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fromthelobby.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.fromthelobby.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Affinity3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affinity Technology (The Lobby), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Affinity Technology (The Lobby)
provider_slug: affinity3
slug: affinity3-domain-security
source_filename: affinity3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fromthelobby.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fromthelobby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinity3/refs/heads/main/security/affinity3-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Influencer Marketing
- Creator Economy
- User Generated Content
- Marketing
- E-Commerce
- Social Media
- Shopify
- Direct to Consumer
---
