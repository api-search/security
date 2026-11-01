---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dollea.de
  spf: true
hosts:
- cert_expires: Jan  2 16:59:51 2027 GMT
  host: dollea.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dollea De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dollea-de, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: dollea-de
provider_slug: dollea-de
slug: dollea-de-domain-security
source_filename: dollea-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dollea.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 16:59:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dollea.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dollea-de/security/dollea-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Beauty
- Salon
- Munich
- Cosmetics
- Wellness
---
