---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "hubspot.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pitt.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: wprdc.org
  spf: true
hosts:
- cert_expires: Aug  4 10:22:57 2026 GMT
  host: www.pitt.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 22:03:11 2026 GMT
  host: data.wprdc.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.tycho.pitt.edu
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Pittsburgh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Pittsburgh, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: University of Pittsburgh
provider_slug: university-of-pittsburgh
slug: university-of-pittsburgh-domain-security
source_filename: university-of-pittsburgh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pitt.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  4 10:22:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: data.wprdc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:03:11 2026 GMT\n  hsts: false\n- host: www.tycho.pitt.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: pitt.edu\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"hubspot.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wprdc.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-pittsburgh/refs/heads/main/security/university-of-pittsburgh-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Research Data
- Library
- United States
---
