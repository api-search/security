---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carota.ai
  spf: true
hosts:
- cert_expires: Dec  1 16:35:53 2026 GMT
  host: www.carota.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carota Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carota, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carota
provider_slug: carota
slug: carota-domain-security
source_filename: carota-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carota.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 16:35:53 2026 GMT\n  hsts: false\ndomains:\n- domain: carota.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carota/refs/heads/main/security/carota-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Automotive
- OTA
- SmartMobility
- AIoT
---
