---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sunrays.dev
  spf: true
hosts:
- cert_expires: Dec  6 06:10:58 2026 GMT
  host: sunrays.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sunrays Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sunrays-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: sunrays-dev
provider_slug: sunrays-dev
slug: sunrays-dev-domain-security
source_filename: sunrays-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunrays.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 06:10:58 2026 GMT\n  hsts: false\ndomains:\n- domain: sunrays.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sunrays-dev/security/sunrays-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Booking
- Local-Services
- MCP
- Agent-Callable
- API
---
