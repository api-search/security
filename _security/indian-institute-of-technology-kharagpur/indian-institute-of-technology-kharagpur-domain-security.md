---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iitkgp.ac.in
  spf: false
- caa:
  - 0 issuewild "ssl.com"
  - 0 issuewild "starfieldtech.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: irins.org
  spf: true
hosts:
- host: www.iitkgp.ac.in
  https: false
- host: www.idr.iitkgp.ac.in
  https: false
- cert_expires: Aug 18 11:22:23 2026 GMT
  host: iitkgp.irins.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indian Institute Of Technology Kharagpur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Institute of Technology Kharagpur, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Indian Institute of Technology Kharagpur
provider_slug: indian-institute-of-technology-kharagpur
slug: indian-institute-of-technology-kharagpur-domain-security
source_filename: indian-institute-of-technology-kharagpur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iitkgp.ac.in\n  https: false\n- host: www.idr.iitkgp.ac.in\n  https: false\n- host: iitkgp.irins.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 11:22:23 2026 GMT\n  hsts: false\ndomains:\n- domain: iitkgp.ac.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: irins.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indian-institute-of-technology-kharagpur/refs/heads/main/security/indian-institute-of-technology-kharagpur-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Institutional Repository
- DSpace
- India
---
