---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: motionspec.dev
  spf: true
hosts:
- cert_expires: Feb  1 18:45:57 2027 GMT
  host: motionspec.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MotionSpec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MotionSpec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MotionSpec
provider_slug: motionspec-dev
slug: motionspec-dev-domain-security
source_filename: motionspec-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motionspec.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 18:45:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: motionspec.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/motionspec-dev/security/motionspec-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- MotionSpec
- Accessibility
- CSS
- Web Agencies
- Open Source
---
