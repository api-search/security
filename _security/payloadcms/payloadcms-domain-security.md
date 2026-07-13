---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payloadcms.com
  spf: true
hosts:
- cert_expires: Sep 24 16:54:22 2026 GMT
  host: payloadcms.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payloadcms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payload CMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Payload CMS
provider_slug: payloadcms
slug: payloadcms-domain-security
source_filename: payloadcms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payloadcms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:54:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: payloadcms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payloadcms/refs/heads/main/security/payloadcms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Headless CMS
- Content Management
- REST API
- GraphQL
- Next.js
- Open Source
- Self-Hosted
- TypeScript
---
