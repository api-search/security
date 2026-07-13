---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: findwork.dev
  spf: true
hosts:
- cert_expires: Oct  4 05:09:00 2026 GMT
  host: findwork.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Findwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Findwork, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Findwork
provider_slug: findwork
slug: findwork-domain-security
source_filename: findwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findwork.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:09:00 2026 GMT\n  hsts: null\ndomains:\n- domain: findwork.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findwork/refs/heads/main/security/findwork-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Jobs
- Public APIs
---
