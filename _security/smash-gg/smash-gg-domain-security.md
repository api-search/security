---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smash.gg
  spf: true
hosts:
- cert_expires: Jan  4 07:14:17 2027 GMT
  host: www.smash.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smash Gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smashgg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smashgg
provider_slug: smash-gg
slug: smash-gg-domain-security
source_filename: smash-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smash.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 07:14:17 2027 GMT\n  hsts: false\ndomains:\n- domain: smash.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/smash-gg/security/smash-gg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
