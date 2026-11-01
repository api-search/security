---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ai-ways.eu
  spf: true
hosts:
- cert_expires: Jan  2 16:53:08 2027 GMT
  host: ai-ways.eu
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiways Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aiways, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aiways
provider_slug: aiways
slug: aiways-domain-security
source_filename: aiways-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-ways.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 16:53:08 2027 GMT\n  hsts: false\ndomains:\n- domain: ai-ways.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aiways/security/aiways-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Electric Vehicles
- Automotive
- EV
- Mobility
- Manufacturer
---
