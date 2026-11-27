---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lockinplanner.com
  spf: false
hosts:
- cert_expires: Jan  5 14:52:44 2027 GMT
  host: lockinplanner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lock In Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lock In, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Lock In
provider_slug: lockinplanner-com
slug: lockinplanner-com-domain-security
source_filename: lockinplanner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lockinplanner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 14:52:44 2027 GMT\n  hsts: false\ndomains:\n- domain: lockinplanner.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lockinplanner-com/security/lockinplanner-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EdTech
- Education
- Study Planner
- Schools
- Research
---
