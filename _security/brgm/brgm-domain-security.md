---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brgm.fr
  spf: true
hosts:
- cert_expires: Feb  6 13:15:02 2027 GMT
  host: www.brgm.fr
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brgm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRGM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BRGM
provider_slug: brgm
slug: brgm-domain-security
source_filename: brgm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brgm.fr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 13:15:02 2027 GMT\n  hsts: false\ndomains:\n- domain: brgm.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/brgm/security/brgm-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Geology
- EarthScience
- PublicService
- France
---
