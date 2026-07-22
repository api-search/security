---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oneok.com
  spf: true
hosts:
- cert_expires: Aug 17 05:53:40 2026 GMT
  host: www.oneok.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oneok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ONEOK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ONEOK
provider_slug: oneok
slug: oneok-domain-security
source_filename: oneok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oneok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 05:53:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oneok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneok/refs/heads/main/security/oneok-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Energy
- Natural Gas
---
