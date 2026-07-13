---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tcd.ie
  spf: true
hosts:
- cert_expires: Aug  1 10:36:50 2026 GMT
  host: www.tcd.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 10:36:50 2026 GMT
  host: digitalcollections.tcd.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trinity College Dublin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trinity College Dublin, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trinity College Dublin
provider_slug: trinity-college-dublin
slug: trinity-college-dublin-domain-security
source_filename: trinity-college-dublin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tcd.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 10:36:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: digitalcollections.tcd.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 10:36:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tcd.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trinity-college-dublin/refs/heads/main/security/trinity-college-dublin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Ireland
- Library
- Repository
- Open Access
- IIIF
- OAI-PMH
---
