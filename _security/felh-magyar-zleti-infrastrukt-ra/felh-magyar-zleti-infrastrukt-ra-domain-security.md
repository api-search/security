---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: felho.hu
  spf: false
hosts:
- cert_expires: Oct 22 12:48:49 2026 GMT
  host: felho.hu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Felh Magyar Zleti Infrastrukt Ra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Felhő — Magyar üzleti infrastruktúra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Felhő — Magyar üzleti infrastruktúra
provider_slug: felh-magyar-zleti-infrastrukt-ra
slug: felh-magyar-zleti-infrastrukt-ra-domain-security
source_filename: felh-magyar-zleti-infrastrukt-ra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: felho.hu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 12:48:49 2026 GMT\n  hsts: false\ndomains:\n- domain: felho.hu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/felh-magyar-zleti-infrastrukt-ra/refs/heads/main/security/felh-magyar-zleti-infrastrukt-ra-domain-security.yml
summary_line: TLSv1.3
tags:
- Company Data
- Business Verification
- Domains
- WHOIS/RDAP
- Hungary
- Registry Data
- Financial Data
---
