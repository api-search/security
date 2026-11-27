---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mpshop.su
  spf: true
hosts:
- cert_expires: Jan 30 00:37:21 2027 GMT
  host: mpshop.su
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MPSHOP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MPSHOP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MPSHOP
provider_slug: mpshop-su
slug: mpshop-su-domain-security
source_filename: mpshop-su-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mpshop.su\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 00:37:21 2027 GMT\n  hsts: false\ndomains:\n- domain: mpshop.su\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mpshop-su/security/mpshop-su-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
