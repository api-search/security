---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kiki.social
  spf: false
hosts:
- cert_expires: Nov 25 14:46:17 2026 GMT
  host: kiki.social
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kiki Social Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kiki
provider_slug: kiki-social
slug: kiki-social-domain-security
source_filename: kiki-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kiki.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 14:46:17 2026 GMT\n  hsts: false\ndomains:\n- domain: kiki.social\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kiki-social/security/kiki-social-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Social
- Mobile
- Networking
- Community
---
