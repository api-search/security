---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: moqi.fr
  spf: true
hosts:
- cert_expires: Jan 23 18:42:19 2027 GMT
  host: moqi.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moqi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moqi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Moqi
provider_slug: moqi-fr
slug: moqi-fr-domain-security
source_filename: moqi-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moqi.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 18:42:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: moqi.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/moqi-fr/security/moqi-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
