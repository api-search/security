---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vervemotion.com
  spf: true
hosts:
- cert_expires: Sep  3 17:26:33 2026 GMT
  host: vervemotion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verve Motion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verve Motion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Verve Motion
provider_slug: verve-motion
slug: verve-motion-domain-security
source_filename: verve-motion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vervemotion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 17:26:33 2026 GMT\n  hsts: false\ndomains:\n- domain: vervemotion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verve-motion/refs/heads/main/security/verve-motion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Wearables
- Worker Safety
- Ergonomics
- Industrial
- Warehousing
- Logistics
- Hardware
- Analytics
---
