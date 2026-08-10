---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quralis.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 08:00:30 2026 GMT
  host: www.quralis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quralis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QurAlis, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QurAlis
provider_slug: quralis
slug: quralis-domain-security
source_filename: quralis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: www.quralis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 08:00:30 2026 GMT\n  hsts: false\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: quralis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quralis/refs/heads/main/security/quralis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Neurology
- Neurodegenerative Disease
- ALS
- Precision Medicine
- Clinical Trials
- Drug Development
- Healthcare
---
