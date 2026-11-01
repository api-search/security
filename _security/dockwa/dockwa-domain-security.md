---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dockwa.com
  spf: true
hosts:
- cert_expires: Dec 30 16:17:31 2026 GMT
  host: dockwa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dockwa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dockwa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dockwa
provider_slug: dockwa
slug: dockwa-domain-security
source_filename: dockwa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dockwa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 16:17:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dockwa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dockwa/security/dockwa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marina
- Boating
- Software
- Software-as-a-Service
- Marketplace
---
