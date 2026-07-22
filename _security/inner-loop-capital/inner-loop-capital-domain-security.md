---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: innerloopcap.com
  spf: true
hosts:
- cert_expires: Sep 25 05:18:24 2026 GMT
  host: www.innerloopcap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inner Loop Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inner Loop Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inner Loop Capital
provider_slug: inner-loop-capital
slug: inner-loop-capital-domain-security
source_filename: inner-loop-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.innerloopcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:18:24 2026 GMT\n  hsts: false\ndomains:\n- domain: innerloopcap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inner-loop-capital/refs/heads/main/security/inner-loop-capital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
