---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oomnitza.com
  spf: true
hosts:
- cert_expires: Oct  3 15:29:51 2026 GMT
  host: www.oomnitza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oomnitza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oomnitza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oomnitza
provider_slug: oomnitza
slug: oomnitza-domain-security
source_filename: oomnitza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oomnitza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:29:51 2026 GMT\n  hsts: false\ndomains:\n- domain: oomnitza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oomnitza/refs/heads/main/security/oomnitza-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IT Asset Management
- SaaS Management
---
