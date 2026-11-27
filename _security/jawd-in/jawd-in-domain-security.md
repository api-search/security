---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jawd.in
  spf: false
hosts:
- cert_expires: Jan  2 17:20:48 2027 GMT
  host: jawd.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JAWD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JAWD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: JAWD
provider_slug: jawd-in
slug: jawd-in-domain-security
source_filename: jawd-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jawd.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 17:20:48 2027 GMT\n  hsts: false\ndomains:\n- domain: jawd.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jawd-in/security/jawd-in-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Health
- Silicone
- India
- Jaw Trainer
---
