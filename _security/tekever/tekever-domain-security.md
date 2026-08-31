---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tekever.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.tekever.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tekever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tekever, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tekever
provider_slug: tekever
slug: tekever-domain-security
source_filename: tekever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tekever.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tekever.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekever/refs/heads/main/security/tekever-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Defense
- Defence Technology
- Unmanned Aerial Systems
- Drones
- ISR
- Intelligence Surveillance Reconnaissance
- Maritime Surveillance
- Satellite
- Synthetic Aperture Radar
- Electronic Warfare
- AI Autonomy
- AR3
- AR5
- ARX
- ATLAS
- Portugal
- United Kingdom
- Ukraine
---
