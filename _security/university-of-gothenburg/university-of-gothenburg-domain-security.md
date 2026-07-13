---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gu.se
  spf: true
hosts:
- cert_expires: Sep  2 07:28:29 2026 GMT
  host: www.gu.se
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 00:22:42 2026 GMT
  host: gupea.ub.gu.se
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Gothenburg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Gothenburg, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Gothenburg
provider_slug: university-of-gothenburg
slug: university-of-gothenburg-domain-security
source_filename: university-of-gothenburg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gu.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 07:28:29 2026 GMT\n  hsts: false\n- host: gupea.ub.gu.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:22:42 2026 GMT\n  hsts: false\ndomains:\n- domain: gu.se\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/security/university-of-gothenburg-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Sweden
- Research
- Open Data
- Library
- OAI-PMH
---
