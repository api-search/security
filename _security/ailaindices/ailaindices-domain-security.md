---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: opal-ai.com
  spf: true
hosts:
- cert_expires: Jan 11 03:53:46 2027 GMT
  host: www.opal-ai.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ailaindices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OPALai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OPALai
provider_slug: ailaindices
slug: ailaindices-domain-security
source_filename: ailaindices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opal-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 03:53:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: opal-ai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ailaindices/security/ailaindices-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Spatial Analytics
- Fire-Intelligence
- Urban Planning
- 3D Scanning
---
