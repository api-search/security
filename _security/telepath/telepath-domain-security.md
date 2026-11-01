---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telepath.computer
  spf: true
hosts:
- cert_expires: Dec 11 01:01:24 2026 GMT
  host: telepath.computer
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Telepath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telepath, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Telepath
provider_slug: telepath
slug: telepath-domain-security
source_filename: telepath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telepath.computer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 01:01:24 2026 GMT\n  hsts: false\ndomains:\n- domain: telepath.computer\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/telepath/security/telepath-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software
- Interface
- AI
- Startup
---
