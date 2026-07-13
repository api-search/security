---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ca.gov
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: globalprivacycontrol.org
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: oag.ca.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 22 23:56:52 2026 GMT
  host: globalprivacycontrol.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  5 23:59:59 2026 GMT
  host: iabtechlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ccpa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CCPA (California Consumer Privacy Act), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CCPA (California Consumer Privacy Act)
provider_slug: ccpa
slug: ccpa-domain-security
source_filename: ccpa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oag.ca.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: globalprivacycontrol.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: iabtechlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ca.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: globalprivacycontrol.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccpa/refs/heads/main/security/ccpa-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- CPRA
- California
- Compliance
- Data Protection
- Data Subject Rights
- Legal
- Privacy
- Regulation
---
