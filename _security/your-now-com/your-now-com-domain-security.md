---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: your-now.com
  spf: true
hosts:
- cert_expires: Dec 26 22:03:10 2026 GMT
  host: www.your-now.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Your Now Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FREE NOW, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FREE NOW
provider_slug: your-now-com
slug: your-now-com-domain-security
source_filename: your-now-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.your-now.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 22:03:10 2026 GMT\n  hsts: false\ndomains:\n- domain: your-now.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/your-now-com/security/your-now-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Mobility
- Car Sharing
- Ride Hailing
- Electric Charging
---
