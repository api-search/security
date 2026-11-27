---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: northwestern.edu
  spf: true
hosts:
- cert_expires: May 28 10:20:10 2027 GMT
  host: northwestern.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Northwestern University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northwestern University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Northwestern University
provider_slug: northwestern-edu
slug: northwestern-edu-domain-security
source_filename: northwestern-edu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: northwestern.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: May 28 10:20:10 2027 GMT\n  hsts: false\ndomains:\n- domain: northwestern.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/northwestern-edu/security/northwestern-edu-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- University
- Research
- Illinois
- Private
---
