---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wayray.com
  spf: true
hosts:
- cert_expires: Nov 19 07:22:22 2026 GMT
  host: wayray.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wayray Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WayRay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: WayRay
provider_slug: wayray
slug: wayray-domain-security
source_filename: wayray-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wayray.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 07:22:22 2026 GMT\n  hsts: false\ndomains:\n- domain: wayray.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayray/refs/heads/main/security/wayray-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Automotive
- Augmented Reality
- Holographic Display
- Deep Tech
- Head-Up Display
- Switzerland
- Defunct
---
