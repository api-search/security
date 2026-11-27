---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tenken.co
  spf: true
hosts:
- cert_expires: Jan 21 04:38:42 2027 GMT
  host: tenken.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tenken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenken, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tenken
provider_slug: tenken-co
slug: tenken-co-domain-security
source_filename: tenken-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tenken.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 04:38:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tenken.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tenken-co/security/tenken-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
