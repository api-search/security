---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tautulli.com
  spf: true
hosts:
- cert_expires: Dec 26 10:18:43 2026 GMT
  host: tautulli.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tautulli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tautulli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Tautulli
provider_slug: tautulli
slug: tautulli-domain-security
source_filename: tautulli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tautulli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 10:18:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: tautulli.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tautulli/security/tautulli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Monitoring
- Plex
- Open-Source
- Analytics
---
