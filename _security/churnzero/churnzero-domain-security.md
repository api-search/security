---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: churnzero.com
  spf: true
hosts:
- cert_expires: Jan 17 00:24:14 2027 GMT
  host: churnzero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Churnzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChurnZero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChurnZero
provider_slug: churnzero
slug: churnzero-domain-security
source_filename: churnzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: churnzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 00:24:14 2027 GMT\n  hsts: null\ndomains:\n- domain: churnzero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/churnzero/security/churnzero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Customer Success
- AI
- SaaS
- Analytics
---
