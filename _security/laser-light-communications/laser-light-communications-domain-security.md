---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: laserlightcomms.com
  spf: true
hosts:
- cert_expires: Oct 18 12:32:32 2026 GMT
  host: www.laserlightcomms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laser Light Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laser Light Communications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Laser Light Communications
provider_slug: laser-light-communications
slug: laser-light-communications-domain-security
source_filename: laser-light-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laserlightcomms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:32:32 2026 GMT\n  hsts: false\ndomains:\n- domain: laserlightcomms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laser-light-communications/refs/heads/main/security/laser-light-communications-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telecommunications
- Networking
- Optical Networking
- Satellite
- Subsea Cable
- Data Centers
- Connectivity
- Infrastructure
- Space
---
