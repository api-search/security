---
description: ''
domains:
- caa:
  - latlong-prod-alb-latlong-ai-1620661566.ap-south-1.elb.amazonaws.com.
  dmarc: false
  dnssec: true
  domain: latlong.ai
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: latlong.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LatLong AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LatLong AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: LatLong AI
provider_slug: latlong-ai
slug: latlong-ai-domain-security
source_filename: latlong-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latlong.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: latlong.ai\n  dnssec: true\n  caa:\n  - latlong-prod-alb-latlong-ai-1620661566.ap-south-1.elb.amazonaws.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/latlong-ai/security/latlong-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Mapping
- Analytics
- Automobile
- BFSI
- Logistics
---
