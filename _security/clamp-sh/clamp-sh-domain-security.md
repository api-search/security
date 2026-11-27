---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clamp.sh
  spf: false
hosts:
- cert_expires: Dec 24 16:35:03 2026 GMT
  host: clamp.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clamp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Clamp
provider_slug: clamp-sh
slug: clamp-sh-domain-security
source_filename: clamp-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clamp.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 16:35:03 2026 GMT\n  hsts: false\ndomains:\n- domain: clamp.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clamp-sh/security/clamp-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Analytics
- Dashboards
- Artificial Intelligence
- Metrics
- Monitoring
---
