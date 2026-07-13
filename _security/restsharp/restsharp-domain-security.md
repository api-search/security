---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: restsharp.dev
  spf: false
hosts:
- cert_expires: Sep 13 23:03:37 2026 GMT
  host: restsharp.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restsharp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RestSharp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RestSharp
provider_slug: restsharp
slug: restsharp-domain-security
source_filename: restsharp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restsharp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:03:37 2026 GMT\n  hsts: false\ndomains:\n- domain: restsharp.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restsharp/refs/heads/main/security/restsharp-domain-security.yml
summary_line: TLSv1.3
tags:
- .NET
- Apache License
- C#
- HTTP Client
- NuGet
- Open Source
- SDKs
---
