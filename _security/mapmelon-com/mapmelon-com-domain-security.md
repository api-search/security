---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mapmelon.com
  spf: true
hosts:
- cert_expires: Feb  1 04:49:11 2027 GMT
  host: mapmelon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mapmelon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mapmelon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mapmelon
provider_slug: mapmelon-com
slug: mapmelon-com-domain-security
source_filename: mapmelon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapmelon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 04:49:11 2027 GMT\n  hsts: false\ndomains:\n- domain: mapmelon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mapmelon-com/security/mapmelon-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Co-Living
- Remote Work
- Community
- Travel
- Housing
---
