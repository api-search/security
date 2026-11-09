---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adradarmcp.cloud
  spf: true
hosts:
- cert_expires: Jan  7 07:25:38 2027 GMT
  host: adradarmcp.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adradarmcp Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdRadar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AdRadar
provider_slug: adradarmcp-cloud
slug: adradarmcp-cloud-domain-security
source_filename: adradarmcp-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adradarmcp.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 07:25:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adradarmcp.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/adradarmcp-cloud/security/adradarmcp-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AdTech
- Artificial Intelligence
- Advertising
- Meta
- TikTok
---
