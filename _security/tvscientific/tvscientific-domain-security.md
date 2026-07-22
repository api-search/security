---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tvscientific.com
  spf: true
hosts:
- cert_expires: Sep 20 00:38:26 2026 GMT
  host: tvscientific.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvscientific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tvscientific, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tvscientific
provider_slug: tvscientific
slug: tvscientific-domain-security
source_filename: tvscientific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tvscientific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:38:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tvscientific.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvscientific/refs/heads/main/security/tvscientific-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Connected TV
- CTV
- Streaming
- Performance Marketing
- AdTech
- Measurement
---
