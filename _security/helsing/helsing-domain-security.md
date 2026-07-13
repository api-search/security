---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: helsing.ai
  spf: true
hosts:
- cert_expires: Sep 22 12:15:53 2026 GMT
  host: helsing.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helsing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helsing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Helsing
provider_slug: helsing
slug: helsing-domain-security
source_filename: helsing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helsing.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:15:53 2026 GMT\n  hsts: null\ndomains:\n- domain: helsing.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helsing/refs/heads/main/security/helsing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Defense AI
- European Defense
- Autonomy
- Loitering Munitions
- Underwater Autonomy
- Electronic Warfare
- AI Fighter Pilot
- Sovereign AI
---
