---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jellystat.com
  spf: false
hosts:
- cert_expires: Dec 25 09:52:30 2026 GMT
  host: jellystat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jellystat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jellystat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jellystat
provider_slug: jellystat
slug: jellystat-domain-security
source_filename: jellystat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jellystat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 09:52:30 2026 GMT\n  hsts: false\ndomains:\n- domain: jellystat.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jellystat/security/jellystat-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Analytics
- OpenSource
- Media
- Jellyfin
---
