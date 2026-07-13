---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecoledesponts.fr
  spf: true
- caa:
  - 0 issue "harica.gr"
  - 0 issuewild "harica.gr"
  - 0 iodef "mailto:ccsd-tech@ccsd.cnrs.fr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hal.science
  spf: true
hosts:
- cert_expires: Aug 14 13:13:51 2026 GMT
  host: ecoledesponts.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 12:15:53 2026 GMT
  host: enpc.hal.science
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
name: Ecole Des Ponts Paristech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for École des Ponts ParisTech, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: École des Ponts ParisTech
provider_slug: ecole-des-ponts-paristech
slug: ecole-des-ponts-paristech-domain-security
source_filename: ecole-des-ponts-paristech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecoledesponts.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 13:13:51 2026 GMT\n  hsts: false\n- host: enpc.hal.science\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:15:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.archives-ouvertes.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ecoledesponts.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hal.science\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"harica.gr\"\n  - 0 iodef \"mailto:ccsd-tech@ccsd.cnrs.fr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecole-des-ponts-paristech/refs/heads/main/security/ecole-des-ponts-paristech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Engineering
- Research
- Open Access
- Open Data
- Library
- OAI-PMH
- France
---
