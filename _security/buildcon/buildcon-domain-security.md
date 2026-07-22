---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: buildcontech.com
  spf: false
hosts:
- cert_expires: Sep 10 23:26:37 2026 GMT
  host: www.buildcontech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buildcon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildcon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Buildcon
provider_slug: buildcon
slug: buildcon-domain-security
source_filename: buildcon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buildcontech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:26:37 2026 GMT\n  hsts: false\ndomains:\n- domain: buildcontech.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildcon/refs/heads/main/security/buildcon-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Construction
- Logistics
- Construction Technology
- Project Management
- Warehouse Management
- SaaS
- Digitalisation
---
