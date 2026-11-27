---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: locus-intelligence.com
  spf: true
hosts:
- cert_expires: Feb  3 18:43:30 2027 GMT
  host: locus-intelligence.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Locus Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Locus Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Locus Intelligence
provider_slug: locus-intelligence-com
slug: locus-intelligence-com-domain-security
source_filename: locus-intelligence-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: locus-intelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 18:43:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: locus-intelligence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/locus-intelligence-com/security/locus-intelligence-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- SEO
- Lead Generation
- Multi-Location
- Platform
---
