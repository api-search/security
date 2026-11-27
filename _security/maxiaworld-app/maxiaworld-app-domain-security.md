---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: maxiaworld.app
  spf: true
hosts:
- cert_expires: Dec 26 13:16:29 2026 GMT
  host: maxiaworld.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MaxiaBat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaxiaBat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: MaxiaBat
provider_slug: maxiaworld-app
slug: maxiaworld-app-domain-security
source_filename: maxiaworld-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maxiaworld.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 13:16:29 2026 GMT\n  hsts: false\ndomains:\n- domain: maxiaworld.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/maxiaworld-app/security/maxiaworld-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- B2B
- Construction
- Project Management
- Software
---
