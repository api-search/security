---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zenoss.com
  spf: true
hosts:
- cert_expires: Oct  1 06:51:00 2026 GMT
  host: www.zenoss.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenoss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenoss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zenoss
provider_slug: zenoss
slug: zenoss-domain-security
source_filename: zenoss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenoss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:51:00 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: zenoss.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenoss/refs/heads/main/security/zenoss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Monitoring
---
