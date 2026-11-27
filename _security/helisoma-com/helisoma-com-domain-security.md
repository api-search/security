---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helisoma.com
  spf: true
hosts:
- cert_expires: Dec 14 15:39:07 2026 GMT
  host: helisoma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Helisoma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helisoma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Helisoma
provider_slug: helisoma-com
slug: helisoma-com-domain-security
source_filename: helisoma-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helisoma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 15:39:07 2026 GMT\n  hsts: false\ndomains:\n- domain: helisoma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/helisoma-com/security/helisoma-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- DNA
- Wellness
- Artificial Intelligence
- Health
- Free
---
