---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upm.edu.my
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: upm.edu.my
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: psasir.upm.edu.my
  https: false
- cert_expires: Sep 21 09:37:09 2026 GMT
  host: idf.upm.edu.my
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universiti Putra Malaysia, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Universiti Putra Malaysia
provider_slug: upm
slug: upm-domain-security
source_filename: upm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upm.edu.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: psasir.upm.edu.my\n  https: false\n- host: idf.upm.edu.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:37:09 2026 GMT\n  hsts: null\ndomains:\n- domain: upm.edu.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upm/refs/heads/main/security/upm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- Identity
- Malaysia
---
