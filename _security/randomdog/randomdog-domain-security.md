---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: random.dog
  spf: false
hosts:
- cert_expires: Oct  3 15:36:01 2026 GMT
  host: random.dog
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Randomdog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RandomDog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RandomDog
provider_slug: randomdog
slug: randomdog-domain-security
source_filename: randomdog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: random.dog\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 15:36:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: random.dog\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/randomdog/refs/heads/main/security/randomdog-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Animals
- Public APIs
---
