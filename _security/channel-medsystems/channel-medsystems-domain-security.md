---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cerene.com
  spf: true
hosts:
- cert_expires: Nov 15 16:15:53 2026 GMT
  host: www.cerene.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Channel Medsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerene, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cerene
provider_slug: channel-medsystems
slug: channel-medsystems-domain-security
source_filename: channel-medsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cerene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 16:15:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cerene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channel-medsystems/refs/heads/main/security/channel-medsystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HealthTech
- Cryotherapy
- Women's Health
- Medical Devices
- FDA Cleared
---
