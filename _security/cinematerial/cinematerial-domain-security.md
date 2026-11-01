---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cinematerial.com
  spf: true
hosts:
- cert_expires: Jan  4 20:07:06 2027 GMT
  host: cinematerial.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cinematerial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CineMaterial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CineMaterial
provider_slug: cinematerial
slug: cinematerial-domain-security
source_filename: cinematerial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cinematerial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 20:07:06 2027 GMT\n  hsts: null\ndomains:\n- domain: cinematerial.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cinematerial/security/cinematerial-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Media
- Archives
- Movies
- Community
---
