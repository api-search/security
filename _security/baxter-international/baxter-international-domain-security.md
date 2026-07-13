---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: baxter.com
  spf: true
hosts:
- cert_expires: Sep 29 06:46:40 2026 GMT
  host: www.baxter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baxter International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baxter International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Baxter International
provider_slug: baxter-international
slug: baxter-international-domain-security
source_filename: baxter-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baxter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:46:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: baxter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baxter-international/refs/heads/main/security/baxter-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Devices
- Infusion Pumps
- Patient Monitoring
- Connected Health
- Fortune 500
---
