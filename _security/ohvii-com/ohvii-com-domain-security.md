---
description: ''
domains:
- caa:
  - 5x276zui.up.railway.app.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ohvii.com
  spf: true
hosts:
- cert_expires: Jan  7 01:28:06 2027 GMT
  host: ohvii.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ohvii-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ohvii-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ohvii-com
provider_slug: ohvii-com
slug: ohvii-com-domain-security
source_filename: ohvii-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohvii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 01:28:06 2027 GMT\n  hsts: null\ndomains:\n- domain: ohvii.com\n  dnssec: true\n  caa:\n  - 5x276zui.up.railway.app.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ohvii-com/security/ohvii-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
