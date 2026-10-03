---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bouldervape.com
  spf: true
hosts:
- cert_expires: Dec 17 21:12:00 2026 GMT
  host: bouldervape.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boulder International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boulder International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boulder International
provider_slug: boulder-international
slug: boulder-international-domain-security
source_filename: boulder-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bouldervape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 21:12:00 2026 GMT\n  hsts: false\ndomains:\n- domain: bouldervape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boulder-international/refs/heads/main/security/boulder-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- vaping
- electronics
- manufacturing
- USA
---
