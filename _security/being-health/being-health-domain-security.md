---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beinghealth.co
  spf: true
hosts:
- cert_expires: Nov  1 07:34:06 2026 GMT
  host: www.beinghealth.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Being Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Being Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Being Health
provider_slug: being-health
slug: being-health-domain-security
source_filename: being-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beinghealth.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 07:34:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beinghealth.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/being-health/refs/heads/main/security/being-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MentalHealth
- Psychiatry
- Wellness
- Telehealth
- NewYork
---
