---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kubb.studio
  spf: true
hosts:
- cert_expires: Dec 18 02:45:01 2026 GMT
  host: kubb.studio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kubb Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubb Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kubb Studio
provider_slug: kubb-studio
slug: kubb-studio-domain-security
source_filename: kubb-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubb.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 02:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubb.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kubb-studio/security/kubb-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Code Generation
- OpenAPI
- TypeScript
- SDK Generation
- Developer Tools
- API Client
- Zod
- TanStack Query
- Mocking
---
