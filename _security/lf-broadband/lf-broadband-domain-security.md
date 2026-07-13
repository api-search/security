---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lfbroadband.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: voltha.org
  spf: false
hosts:
- cert_expires: Sep  6 18:54:28 2026 GMT
  host: lfbroadband.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:15:01 2026 GMT
  host: docs.voltha.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: opennetworking.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lf Broadband Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LF Broadband, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LF Broadband
provider_slug: lf-broadband
slug: lf-broadband-domain-security
source_filename: lf-broadband-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lfbroadband.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.voltha.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:15:01 2026 GMT\n  hsts: false\n- host: opennetworking.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lfbroadband.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: voltha.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lf-broadband/refs/heads/main/security/lf-broadband-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Broadband
- Linux Foundation
- Networking
- Telecom
- PON
- Open Source
- SDN
---
