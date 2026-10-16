---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: raritan.com
  spf: true
hosts:
- cert_expires: Dec 30 00:57:45 2026 GMT
  host: www.raritan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Raritan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raritan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Raritan
provider_slug: raritan
slug: raritan-domain-security
source_filename: raritan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raritan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 00:57:45 2026 GMT\n  hsts: false\ndomains:\n- domain: raritan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raritan/refs/heads/main/security/raritan-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Power Management
- DCIM
- KVM-over-IP
- Data Center
---
