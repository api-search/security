---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: blust.ch
  spf: true
hosts:
- cert_expires: Jan 19 18:43:51 2027 GMT
  host: blust.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blust Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for blust-ch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: blust-ch
provider_slug: blust-ch
slug: blust-ch-domain-security
source_filename: blust-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blust.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 18:43:51 2027 GMT\n  hsts: false\ndomains:\n- domain: blust.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blust-ch/security/blust-ch-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
