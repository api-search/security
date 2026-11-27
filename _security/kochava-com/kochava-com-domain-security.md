---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kochava.com
  spf: true
hosts:
- cert_expires: Dec 30 20:47:36 2026 GMT
  host: kochava.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kochava Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kochava, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kochava
provider_slug: kochava-com
slug: kochava-com-domain-security
source_filename: kochava-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kochava.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 20:47:36 2026 GMT\n  hsts: false\ndomains:\n- domain: kochava.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kochava-com/security/kochava-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Analytics
- Mobile
- Measurements
- Privacy
---
