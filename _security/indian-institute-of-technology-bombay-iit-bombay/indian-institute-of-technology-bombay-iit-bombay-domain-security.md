---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iitb.ac.in
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.iitb.ac.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Indian Institute Of Technology Bombay Iit Bombay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Institute of Technology Bombay (IIT Bombay), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Indian Institute of Technology Bombay (IIT Bombay)
provider_slug: indian-institute-of-technology-bombay-iit-bombay
slug: indian-institute-of-technology-bombay-iit-bombay-domain-security
source_filename: indian-institute-of-technology-bombay-iit-bombay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iitb.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: iitb.ac.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/indian-institute-of-technology-bombay-iit-bombay/security/indian-institute-of-technology-bombay-iit-bombay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- University
- India
- Engineering
- Research
- Company
---
