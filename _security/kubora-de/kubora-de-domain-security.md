---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kubora.de
  spf: true
hosts:
- cert_expires: Jan  3 16:31:25 2027 GMT
  host: kubora.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kubora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kubora
provider_slug: kubora-de
slug: kubora-de-domain-security
source_filename: kubora-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubora.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 16:31:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubora.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kubora-de/security/kubora-de-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Self Storage
- Comparison
- Germany
- Real Estate
- Logistics
---
