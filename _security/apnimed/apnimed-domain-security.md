---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apnimed.com
  spf: true
hosts:
- cert_expires: Oct 13 23:46:08 2026 GMT
  host: apnimed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apnimed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apnimed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apnimed
provider_slug: apnimed
slug: apnimed-domain-security
source_filename: apnimed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apnimed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:46:08 2026 GMT\n  hsts: false\ndomains:\n- domain: apnimed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apnimed/refs/heads/main/security/apnimed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Healthcare
- Life Sciences
- Sleep Medicine
- Clinical Trials
---
