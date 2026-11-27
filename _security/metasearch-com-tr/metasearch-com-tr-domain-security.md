---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: metasearch.com.tr
  spf: true
hosts:
- cert_expires: Feb 16 04:34:25 2027 GMT
  host: metasearch.com.tr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metasearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metasearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Metasearch
provider_slug: metasearch-com-tr
slug: metasearch-com-tr-domain-security
source_filename: metasearch-com-tr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metasearch.com.tr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 04:34:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: metasearch.com.tr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/metasearch-com-tr/security/metasearch-com-tr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Metasearch
- Integration
- Data
---
