---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: statcounter.com
  spf: true
hosts:
- cert_expires: Dec 25 22:39:54 2026 GMT
  host: statcounter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Statcounter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StatCounter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: StatCounter
provider_slug: statcounter
slug: statcounter-domain-security
source_filename: statcounter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statcounter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 22:39:54 2026 GMT\n  hsts: false\ndomains:\n- domain: statcounter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/statcounter/security/statcounter-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Analytics
- Web
- Real-time
- Heatmaps
---
