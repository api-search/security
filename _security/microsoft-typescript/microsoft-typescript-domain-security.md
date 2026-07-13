---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: typescriptlang.org
  spf: false
hosts:
- cert_expires: Sep 29 13:29:52 2026 GMT
  host: www.typescriptlang.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Typescript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft TypeScript, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Microsoft TypeScript
provider_slug: microsoft-typescript
slug: microsoft-typescript-domain-security
source_filename: microsoft-typescript-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.typescriptlang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:29:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: typescriptlang.org\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-typescript/refs/heads/main/security/microsoft-typescript-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compiler
- JavaScript
- Language Tools
- Microsoft
- TypeScript
---
