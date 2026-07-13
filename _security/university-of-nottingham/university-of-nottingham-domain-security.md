---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nottingham.ac.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: worktribe.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.nottingham.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 18:41:19 2026 GMT
  host: nottingham-repository.worktribe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: eprints.nottingham.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Nottingham Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Nottingham, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Nottingham
provider_slug: university-of-nottingham
slug: university-of-nottingham-domain-security
source_filename: university-of-nottingham-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nottingham.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: nottingham-repository.worktribe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:41:19 2026 GMT\n  hsts: null\n- host: eprints.nottingham.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nottingham.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: worktribe.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-nottingham/refs/heads/main/security/university-of-nottingham-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- OAI-PMH
- United Kingdom
---
