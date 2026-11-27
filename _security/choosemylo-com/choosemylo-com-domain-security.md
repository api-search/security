---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: choosemylo.com
  spf: true
hosts:
- cert_expires: Jan  8 21:36:09 2027 GMT
  host: choosemylo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mylo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mylo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mylo
provider_slug: choosemylo-com
slug: choosemylo-com-domain-security
source_filename: choosemylo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: choosemylo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 21:36:09 2027 GMT\n  hsts: false\ndomains:\n- domain: choosemylo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/choosemylo-com/security/choosemylo-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Insurtech
- Insurance Brokerage
- Small Business
- Quotes
- MCP
---
