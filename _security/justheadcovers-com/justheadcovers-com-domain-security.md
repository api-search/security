---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: justheadcovers.com
  spf: true
hosts:
- cert_expires: Jan 24 04:17:10 2027 GMT
  host: justheadcovers.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Just Headcovers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Just Headcovers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Just Headcovers
provider_slug: justheadcovers-com
slug: justheadcovers-com-domain-security
source_filename: justheadcovers-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justheadcovers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 04:17:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: justheadcovers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/justheadcovers-com/security/justheadcovers-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Golf
- E-Commerce
- Marketplace
- Headcovers
- Community
---
