---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rayfit.com
  spf: false
hosts:
- cert_expires: Jan 20 22:50:45 2027 GMT
  host: rayfit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rayfit Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ray, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Ray
provider_slug: rayfit-com
slug: rayfit-com-domain-security
source_filename: rayfit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rayfit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 22:50:45 2027 GMT\n  hsts: false\ndomains:\n- domain: rayfit.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rayfit-com/security/rayfit-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI
- Fitness
- Health
- Personal Trainer
- Wellness
- Company
---
