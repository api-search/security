---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gla.ac.uk
  spf: true
hosts:
- cert_expires: Aug 12 23:27:51 2026 GMT
  host: www.gla.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 23:24:56 2026 GMT
  host: eprints.gla.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:22:57 2026 GMT
  host: researchdata.gla.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Glasgow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Glasgow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Glasgow
provider_slug: university-of-glasgow
slug: university-of-glasgow-domain-security
source_filename: university-of-glasgow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gla.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:27:51 2026 GMT\n  hsts: false\n- host: eprints.gla.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:24:56 2026 GMT\n  hsts: false\n- host: researchdata.gla.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:22:57 2026 GMT\n  hsts: false\ndomains:\n- domain: gla.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-glasgow/refs/heads/main/security/university-of-glasgow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- OAI-PMH
- United Kingdom
- Scotland
---
