---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: getfishbit.com
  spf: true
hosts:
- cert_expires: Sep 28 20:39:54 2026 GMT
  host: getfishbit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fishbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fishbit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Fishbit
provider_slug: fishbit
slug: fishbit-domain-security
source_filename: fishbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfishbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:39:54 2026 GMT\n  hsts: false\ndomains:\n- domain: getfishbit.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fishbit/refs/heads/main/security/fishbit-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Aquarium
- Smart Home
- IoT
- Connected Hardware
- Water Monitoring
- Consumer Electronics
---
