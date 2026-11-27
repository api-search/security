---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: controlflare.com
  spf: true
hosts:
- cert_expires: Dec 18 09:08:29 2026 GMT
  host: controlflare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Controlflare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Controlflare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Controlflare
provider_slug: controlflare-com
slug: controlflare-com-domain-security
source_filename: controlflare-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: controlflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 09:08:29 2026 GMT\n  hsts: false\ndomains:\n- domain: controlflare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/controlflare-com/security/controlflare-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cloudflare
- Cloudflare Workers
- Cost Management
- Budget Caps
- FinOps
- MCP
- Serverless
---
