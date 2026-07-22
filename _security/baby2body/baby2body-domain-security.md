---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bodycollective.group
  spf: true
hosts:
- cert_expires: Sep  4 07:01:17 2026 GMT
  host: bodycollective.group
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baby2Body Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baby2Body, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Baby2Body
provider_slug: baby2body
slug: baby2body-domain-security
source_filename: baby2body-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bodycollective.group\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:01:17 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: bodycollective.group\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baby2body/refs/heads/main/security/baby2body-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Wellness
- Fitness
- Pregnancy
- Women's Health
- Consumer
- Mobile App
---
