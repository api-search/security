---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uantwerpen.be
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: openarchives.org
  spf: false
hosts:
- cert_expires: Nov 13 11:23:08 2026 GMT
  host: www.uantwerpen.be
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.openarchives.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: repository.uantwerpen.be
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Antwerp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Antwerp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Antwerp
provider_slug: university-of-antwerp
slug: university-of-antwerp-domain-security
source_filename: university-of-antwerp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uantwerpen.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 11:23:08 2026 GMT\n  hsts: false\n- host: www.openarchives.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: repository.uantwerpen.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: uantwerpen.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openarchives.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-antwerp/refs/heads/main/security/university-of-antwerp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Library
- Institutional Repository
- OAI-PMH
- Open Data
- Belgium
- Europe
---
