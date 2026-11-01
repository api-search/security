---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: df.eu
  spf: true
hosts:
- cert_expires: Mar  6 09:30:54 2027 GMT
  host: df.eu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domainfactory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DomainFactory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DomainFactory
provider_slug: domainfactory
slug: domainfactory-domain-security
source_filename: domainfactory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: df.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 09:30:54 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: df.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/domainfactory/security/domainfactory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hosting
- Domains
- WebHosting
- SSL
---
