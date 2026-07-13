---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ku.ac.ae
  spf: true
hosts:
- cert_expires: Mar 21 08:16:15 2027 GMT
  host: www.ku.ac.ae
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Khalifa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Khalifa University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Khalifa University
provider_slug: khalifa
slug: khalifa-domain-security
source_filename: khalifa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ku.ac.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 08:16:15 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ku.ac.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/khalifa/refs/heads/main/security/khalifa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Robotics
- United Arab Emirates
- Abu Dhabi
---
