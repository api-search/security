---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: faroz.uz
  spf: false
hosts:
- cert_expires: Jan 20 02:59:44 2027 GMT
  host: faroz.uz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faroz Uz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faroz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Faroz
provider_slug: faroz-uz
slug: faroz-uz-domain-security
source_filename: faroz-uz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faroz.uz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 02:59:44 2027 GMT\n  hsts: false\ndomains:\n- domain: faroz.uz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/faroz-uz/security/faroz-uz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
