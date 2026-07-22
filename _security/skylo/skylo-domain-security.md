---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: skylo.tech
  spf: true
hosts:
- cert_expires: Sep  3 07:07:36 2026 GMT
  host: www.skylo.tech
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skylo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skylo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Skylo
provider_slug: skylo
slug: skylo-domain-security
source_filename: skylo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skylo.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:07:36 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: skylo.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skylo/refs/heads/main/security/skylo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Frontier Tech
- Satellite
- Connectivity
- IoT
- Non-Terrestrial Network
- Direct-to-Device
- Telecommunications
---
