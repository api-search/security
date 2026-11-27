---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: facehunch.com
  spf: false
hosts:
- cert_expires: Dec 20 16:25:09 2026 GMT
  host: facehunch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Facehunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facehunch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Facehunch
provider_slug: facehunch-com
slug: facehunch-com-domain-security
source_filename: facehunch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facehunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 16:25:09 2026 GMT\n  hsts: false\ndomains:\n- domain: facehunch.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/facehunch-com/security/facehunch-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Face Recognition
- Reverse Image Search
- Privacy
- Security
- Artificial Intelligence
---
