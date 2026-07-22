---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realnetworks.com
  spf: true
hosts:
- cert_expires: Oct  6 22:00:44 2026 GMT
  host: www.realnetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realnetworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealNetworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RealNetworks
provider_slug: realnetworks
slug: realnetworks-domain-security
source_filename: realnetworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realnetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:00:44 2026 GMT\n  hsts: false\ndomains:\n- domain: realnetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realnetworks/refs/heads/main/security/realnetworks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Facial Recognition
- Computer Vision
- Messaging Security
- CPaaS
- Gaming
- Media
- Artificial Intelligence
---
