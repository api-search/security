---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: myprivacyagent.com
  spf: false
hosts:
- cert_expires: Dec 27 10:58:42 2026 GMT
  host: myprivacyagent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: My Privacy Agent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for My Privacy Agent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: My Privacy Agent
provider_slug: myprivacyagent-com
slug: myprivacyagent-com-domain-security
source_filename: myprivacyagent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myprivacyagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 10:58:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: myprivacyagent.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/myprivacyagent-com/security/myprivacyagent-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Personal Information Removal
- Data Broker Opt‑out
---
