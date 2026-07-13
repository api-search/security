---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asq.org
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: minitab.com
  spf: true
hosts:
- cert_expires: Sep 13 18:47:35 2026 GMT
  host: www.asq.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 18:47:35 2026 GMT
  host: asq.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.minitab.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Six Sigma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Six Sigma, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Six Sigma
provider_slug: six-sigma
slug: six-sigma-domain-security
source_filename: six-sigma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asq.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:47:35 2026 GMT\n  hsts: false\n- host: asq.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:47:35 2026 GMT\n  hsts: false\n- host: www.minitab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: asq.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: minitab.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/six-sigma/refs/heads/main/security/six-sigma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quality Management
- Process Improvement
- Lean Manufacturing
- Business Excellence
- Statistical Analysis
- DMAIC
- Operational Excellence
---
