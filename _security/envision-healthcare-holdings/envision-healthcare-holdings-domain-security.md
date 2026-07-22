---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evhc.net
  spf: false
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.evhc.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envision Healthcare Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envision Healthcare Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Envision Healthcare Holdings
provider_slug: envision-healthcare-holdings
slug: envision-healthcare-holdings-domain-security
source_filename: envision-healthcare-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evhc.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: evhc.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envision-healthcare-holdings/refs/heads/main/security/envision-healthcare-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Physician Services
- Ambulatory Surgery
---
