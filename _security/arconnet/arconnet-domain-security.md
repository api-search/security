---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arconnet.com
  spf: true
hosts:
- cert_expires: Nov 20 04:30:40 2026 GMT
  host: www.arconnet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arconnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARCON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ARCON
provider_slug: arconnet
slug: arconnet-domain-security
source_filename: arconnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arconnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 04:30:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arconnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arconnet/refs/heads/main/security/arconnet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Identity
- Access Control
- Enterprise
---
