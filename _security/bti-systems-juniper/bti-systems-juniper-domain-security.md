---
description: ''
domains:
- caa: null
  dmarc: null
  dmarc_policy: null
  dnssec: null
  domain: btisystems.com
  resolves: false
  spf: null
hosts:
- dns_a_records: []
  host: btisystems.com
  hsts: null
  http_status: null
  https: false
  resolves: false
  role: historical-corporate-domain
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Bti Systems Juniper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BTI Systems (Juniper), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BTI Systems (Juniper)
provider_slug: bti-systems-juniper
slug: bti-systems-juniper-domain-security
source_filename: bti-systems-juniper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + HTTPS probe, 2026-07-20\nnote: BTI Systems has no independent operating domain following the 2016 Juniper Networks\n  acquisition. The historical corporate domain btisystems.com no longer resolves. The similarly\n  named bti-systems.com and bti.net are unrelated third-party businesses and are deliberately\n  NOT attributed to this company. Corporate domain security for the acquiring entity is probed\n  in the juniper-networks profile, not here.\nhosts:\n- host: btisystems.com\n  role: historical-corporate-domain\n  dns_a_records: []\n  resolves: false\n  https: false\n  http_status: null\n  tls_version: null\n  hsts: null\ndomains:\n- domain: btisystems.com\n  resolves: false\n  dnssec: null\n  caa: null\n  spf: null\n  dmarc: null\n  dmarc_policy: null\nexcluded_hosts:\n- host: bti-systems.com\n  reason: unrelated IT services company, name collision only\n- host: bti.net\n  reason: unrelated third-party domain, name collision\
  \ only\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bti-systems-juniper/refs/heads/main/security/bti-systems-juniper-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Networking
- Optical Networking
- Packet Optical Transport
- Telecommunications
- Network Management
- SDN
- NFV
- Acquired
---
