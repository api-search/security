---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sorbonne-universite.fr
  spf: true
- caa:
  - 0 iodef "mailto:ccsd-tech@ccsd.cnrs.fr"
  - 0 issuewild "harica.gr"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archives-ouvertes.fr
  spf: true
hosts:
- cert_expires: Aug 24 15:19:19 2026 GMT
  host: www.sorbonne-universite.fr
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 02:37:20 2026 GMT
  host: hal.sorbonne-universite.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 12:16:58 2026 GMT
  host: api.archives-ouvertes.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sorbonne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sorbonne University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sorbonne University
provider_slug: sorbonne
slug: sorbonne-domain-security
source_filename: sorbonne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sorbonne-universite.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:19:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: hal.sorbonne-universite.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:37:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.archives-ouvertes.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sorbonne-universite.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: archives-ouvertes.fr\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:ccsd-tech@ccsd.cnrs.fr\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorbonne/refs/heads/main/security/sorbonne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Open Science
- Research Data
- Open Access
- OAI-PMH
- Dataverse
- France
---
