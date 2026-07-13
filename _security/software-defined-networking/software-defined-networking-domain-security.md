---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opennetworking.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opendaylight.org
  spf: true
hosts:
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: opennetworking.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 03:46:29 2026 GMT
  host: docs.opendaylight.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: wiki.onosproject.org
  https: false
kind: domain-security
layout: security
method: probed
name: Software Defined Networking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software-Defined Networking, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Software-Defined Networking
provider_slug: software-defined-networking
slug: software-defined-networking-domain-security
source_filename: software-defined-networking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opennetworking.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: false\n- host: docs.opendaylight.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:46:29 2026 GMT\n  hsts: false\n- host: wiki.onosproject.org\n  https: false\ndomains:\n- domain: opennetworking.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opendaylight.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-defined-networking/refs/heads/main/security/software-defined-networking-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Infrastructure
- Network Architecture
- Networking
- Virtualization
- SDN
- OpenDaylight
- ONOS
---
