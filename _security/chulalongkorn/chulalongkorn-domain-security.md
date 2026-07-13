---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chula.ac.th
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.chula.ac.th
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 00:56:49 2026 GMT
  host: account.it.chula.ac.th
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  3 06:14:28 2026 GMT
  host: digiverse.chula.ac.th
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chulalongkorn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chulalongkorn University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chulalongkorn University
provider_slug: chulalongkorn
slug: chulalongkorn-domain-security
source_filename: chulalongkorn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chula.ac.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: account.it.chula.ac.th\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 00:56:49 2026 GMT\n  hsts: null\n- host: digiverse.chula.ac.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:14:28 2026 GMT\n  hsts: false\ndomains:\n- domain: chula.ac.th\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chulalongkorn/refs/heads/main/security/chulalongkorn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Thailand
- Identity
- Single Sign-On
- Institutional Repository
- Open Access
- OAI-PMH
---
