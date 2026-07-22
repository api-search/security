---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quokkadev.com
  spf: true
hosts:
- cert_expires: Oct  5 22:44:11 2026 GMT
  host: www.quokkadev.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quokka Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quokka Sports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Quokka Sports
provider_slug: quokka-sports
slug: quokka-sports-domain-security
source_filename: quokka-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quokkadev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:44:11 2026 GMT\n  hsts: false\ndomains:\n- domain: quokkadev.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quokka-sports/refs/heads/main/security/quokka-sports-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
