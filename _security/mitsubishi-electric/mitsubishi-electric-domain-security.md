---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mitsubishielectric.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.mitsubishielectric.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mitsubishi Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitsubishi Electric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mitsubishi Electric
provider_slug: mitsubishi-electric
slug: mitsubishi-electric-domain-security
source_filename: mitsubishi-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mitsubishielectric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mitsubishielectric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitsubishi-electric/refs/heads/main/security/mitsubishi-electric-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Electronics
- Automation
- Energy
- Infrastructure
---
