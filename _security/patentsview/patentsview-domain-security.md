---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: patentsview.org
  spf: true
hosts:
- cert_expires: Sep 18 15:30:49 2026 GMT
  host: patentsview.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patentsview Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PatentsView, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PatentsView
provider_slug: patentsview
slug: patentsview-domain-security
source_filename: patentsview-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patentsview.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 15:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: patentsview.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patentsview/refs/heads/main/security/patentsview-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Patent
- Public APIs
---
