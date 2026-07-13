---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: softwaresuggest.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: datarade.ai
  spf: true
hosts:
- cert_expires: Aug 22 00:29:08 2026 GMT
  host: www.softwaresuggest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 03:09:08 2026 GMT
  host: datarade.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Softwaresuggest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoftwareSuggest, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SoftwareSuggest
provider_slug: softwaresuggest
slug: softwaresuggest-domain-security
source_filename: softwaresuggest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.softwaresuggest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 00:29:08 2026 GMT\n  hsts: false\n- host: datarade.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:09:08 2026 GMT\n  hsts: null\ndomains:\n- domain: softwaresuggest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: datarade.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/softwaresuggest/refs/heads/main/security/softwaresuggest-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Software Discovery
- Business Software
- SaaS
- Software Reviews
- B2B
---
