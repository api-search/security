---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flusia.it
  spf: true
hosts:
- cert_expires: Dec 28 05:58:36 2026 GMT
  host: flusia.it
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flusia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flusia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flusia
provider_slug: flusia-it
slug: flusia-it-domain-security
source_filename: flusia-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flusia.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 05:58:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: flusia.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flusia-it/security/flusia-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Software-as-a-Service
- Italian
- Small Business
---
