---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amcnetworks.com
  spf: true
hosts:
- cert_expires: Sep 26 06:41:04 2026 GMT
  host: www.amcnetworks.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 13:27:18 2026 GMT
  host: affiliate.amcnetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amc Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMC Networks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AMC Networks
provider_slug: amc-networks
slug: amc-networks-domain-security
source_filename: amc-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amcnetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:41:04 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: affiliate.amcnetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:27:18 2026 GMT\n  hsts: false\ndomains:\n- domain: amcnetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amc-networks/refs/heads/main/security/amc-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Streaming
- Cable Television
- Advertising
- Media
- FAST Channels
- Fortune 1000
---
