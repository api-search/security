---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tu-darmstadt.de
  spf: true
hosts:
- cert_expires: Sep  1 14:14:33 2026 GMT
  host: www.tu-darmstadt.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 11:01:17 2026 GMT
  host: tudatalib.ulb.tu-darmstadt.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 08:14:39 2026 GMT
  host: tubiblio.ulb.tu-darmstadt.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Technical University Of Darmstadt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technical University of Darmstadt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Technical University of Darmstadt
provider_slug: technical-university-of-darmstadt
slug: technical-university-of-darmstadt-domain-security
source_filename: technical-university-of-darmstadt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tu-darmstadt.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 14:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tudatalib.ulb.tu-darmstadt.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 11:01:17 2026 GMT\n  hsts: false\n- host: tubiblio.ulb.tu-darmstadt.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 08:14:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tu-darmstadt.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/technical-university-of-darmstadt/refs/heads/main/security/technical-university-of-darmstadt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Library
- OAI-PMH
- DSpace
- Germany
---
