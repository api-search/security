---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xamarin.com
  spf: false
hosts:
- cert_expires: Oct 24 14:04:56 2026 GMT
  host: xamarin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xamarin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xamarin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Xamarin
provider_slug: xamarin
slug: xamarin-domain-security
source_filename: xamarin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xamarin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 14:04:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xamarin.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xamarin/refs/heads/main/security/xamarin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Devops
- Mobile
- Cross-Platform
- DotNet
- SDK
- Microsoft
---
