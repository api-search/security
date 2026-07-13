---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: distillersr.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: evidencepartners.com
  spf: true
hosts:
- cert_expires: Sep 14 11:09:40 2026 GMT
  host: www.distillersr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: v1serv-prod.evidencepartners.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Distillersr Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DistillerSR, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DistillerSR
provider_slug: distillersr-api
slug: distillersr-api-domain-security
source_filename: distillersr-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.distillersr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:09:40 2026 GMT\n  hsts: false\n- host: v1serv-prod.evidencepartners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: distillersr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: evidencepartners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distillersr-api/refs/heads/main/security/distillersr-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Literature Reviews
- Systematic Reviews
- Research
---
