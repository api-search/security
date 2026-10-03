---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: berlinbrands.de
  spf: true
hosts:
- cert_expires: Nov 28 15:20:55 2026 GMT
  host: www.berlinbrands.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Berlin Brands Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Berlin Brands Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Berlin Brands Group
provider_slug: berlin-brands-group
slug: berlin-brands-group-domain-security
source_filename: berlin-brands-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.berlinbrands.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 15:20:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: berlinbrands.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/berlin-brands-group/refs/heads/main/security/berlin-brands-group-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-Commerce
- Consumer Goods
- Berlin
- Holding
---
