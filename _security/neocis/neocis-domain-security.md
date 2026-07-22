---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neocis.com
  spf: true
hosts:
- cert_expires: Aug 23 13:28:48 2026 GMT
  host: neocis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neocis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neocis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neocis
provider_slug: neocis
slug: neocis-domain-security
source_filename: neocis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neocis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 13:28:48 2026 GMT\n  hsts: false\ndomains:\n- domain: neocis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neocis/refs/heads/main/security/neocis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Dental
- Robotics
- Surgery
- Health
- Medical
---
