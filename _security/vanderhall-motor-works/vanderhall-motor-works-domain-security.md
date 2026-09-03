---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vanderhallusa.com
  spf: true
hosts:
- cert_expires: Nov 27 18:13:06 2026 GMT
  host: vanderhallusa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 13:26:52 2026 GMT
  host: portal.vanderhallusa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vanderhall Motor Works Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanderhall Motor Works, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vanderhall Motor Works
provider_slug: vanderhall-motor-works
slug: vanderhall-motor-works-domain-security
source_filename: vanderhall-motor-works-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vanderhallusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 18:13:06 2026 GMT\n  hsts: false\n- host: portal.vanderhallusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 13:26:52 2026 GMT\n  hsts: false\ndomains:\n- domain: vanderhallusa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanderhall-motor-works/refs/heads/main/security/vanderhall-motor-works-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Manufacturing
- Electric Vehicles
- Powersports
- Autocycles
- Dealer Network
- Model Context Protocol
- Utah
---
