---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lfconnectivity.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magmacore.org
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: lfconnectivity.dev
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: magmacore.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 10:32:51 2026 GMT
  host: terragraph.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lf Connectivity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LF Connectivity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LF Connectivity
provider_slug: lf-connectivity
slug: lf-connectivity-domain-security
source_filename: lf-connectivity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lfconnectivity.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: magmacore.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: false\n- host: terragraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:32:51 2026 GMT\n  hsts: false\ndomains:\n- domain: lfconnectivity.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: magmacore.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lf-connectivity/refs/heads/main/security/lf-connectivity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connectivity
- Linux Foundation
- Networking
- Telecom
- Wireless
- 5G
- Open Source
---
