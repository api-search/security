---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: inspirehep.net
  spf: true
hosts:
- cert_expires: Dec 21 02:21:10 2026 GMT
  host: inspirehep.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inspire Hep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INSPIRE HEP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: INSPIRE HEP
provider_slug: inspire-hep
slug: inspire-hep-domain-security
source_filename: inspire-hep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inspirehep.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 02:21:10 2026 GMT\n  hsts: false\ndomains:\n- domain: inspirehep.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inspire-hep/refs/heads/main/security/inspire-hep-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- HighEnergyPhysics
- Research
- Data
- OpenScience
---
