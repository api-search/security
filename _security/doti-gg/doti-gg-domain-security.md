---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doti.gg
  spf: true
hosts:
- cert_expires: Jan 27 20:06:43 2027 GMT
  host: doti.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: D0T1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D0T1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: D0T1
provider_slug: doti-gg
slug: doti-gg-domain-security
source_filename: doti-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doti.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 20:06:43 2027 GMT\n  hsts: false\ndomains:\n- domain: doti.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/doti-gg/security/doti-gg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Content Generation
- Automation
- Marketing
---
