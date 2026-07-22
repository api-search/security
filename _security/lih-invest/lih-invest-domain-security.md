---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lih-invest.com
  spf: true
hosts:
- cert_expires: Mar 12 09:46:23 2027 GMT
  host: www.lih-invest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lih Invest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LIH Healthcare (长和医疗), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LIH Healthcare (长和医疗)
provider_slug: lih-invest
slug: lih-invest-domain-security
source_filename: lih-invest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lih-invest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 09:46:23 2027 GMT\n  hsts: false\ndomains:\n- domain: lih-invest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lih-invest/refs/heads/main/security/lih-invest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Rehabilitation
- Hospitals
- Medical Services
- Healthcare Investment
- Pediatrics
- China
---
