---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: evgo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plugshare.com
  spf: true
hosts:
- cert_expires: Sep  2 00:00:05 2026 GMT
  host: www.evgo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.evgo.com
  https: false
- cert_expires: Sep 28 10:59:49 2026 GMT
  host: developer.plugshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EVgo, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: EVgo
provider_slug: evgo
slug: evgo-domain-security
source_filename: evgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:00:05 2026 GMT\n  hsts: null\n- host: api.evgo.com\n  https: false\n- host: developer.plugshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:59:49 2026 GMT\n  hsts: false\ndomains:\n- domain: evgo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: plugshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evgo/refs/heads/main/security/evgo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Electric Vehicles
- EV Charging
- Charging Stations
- Energy
- Transportation
- Mobility
---
