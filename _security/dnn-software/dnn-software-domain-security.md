---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dnnsoftware.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: dnnsoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dnn Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNN Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DNN Software
provider_slug: dnn-software
slug: dnn-software-domain-security
source_filename: dnn-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dnnsoftware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dnnsoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnn-software/refs/heads/main/security/dnn-software-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Saas
- CMS
- Content Management
- Open Source
- ASP.NET
- .NET
- Web Framework
- DotNetNuke
---
