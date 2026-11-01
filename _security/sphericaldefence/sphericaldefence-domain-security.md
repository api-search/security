---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sphericaldefence.com
  spf: true
hosts:
- cert_expires: Dec  9 17:29:26 2026 GMT
  host: sphericaldefence.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sphericaldefence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spherical Defense, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spherical Defense
provider_slug: sphericaldefence
slug: sphericaldefence-domain-security
source_filename: sphericaldefence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sphericaldefence.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 17:29:26 2026 GMT\n  hsts: false\ndomains:\n- domain: sphericaldefence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/sphericaldefence/security/sphericaldefence-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Cybersecurity
- Artificial Intelligence
- Threat Detection
- Cloud-Native
---
