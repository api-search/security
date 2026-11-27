---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: true
  domain: triphook.me
  spf: true
hosts:
- cert_expires: Jan 18 23:26:11 2027 GMT
  host: triphook.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TripHook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TripHook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TripHook
provider_slug: triphook-me
slug: triphook-me-domain-security
source_filename: triphook-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triphook.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:26:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: triphook.me\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/triphook-me/security/triphook-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Search
- Mood
- Budget
- Community
---
