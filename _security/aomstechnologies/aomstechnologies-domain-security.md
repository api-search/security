---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amstechnologies.com
  spf: true
hosts:
- cert_expires: Dec  7 21:35:24 2026 GMT
  host: amstechnologies.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aomstechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aomstechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aomstechnologies
provider_slug: aomstechnologies
slug: aomstechnologies-domain-security
source_filename: aomstechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amstechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 21:35:24 2026 GMT\n  hsts: false\ndomains:\n- domain: amstechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aomstechnologies/refs/heads/main/security/aomstechnologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Optical
- Thermal Management
- Electronics
- Engineering
- Custom Solutions
---
