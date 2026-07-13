---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ens-lyon.fr
  spf: true
- caa:
  - 0 issuewild "harica.gr"
  - 0 iodef "mailto:ccsd-tech@ccsd.cnrs.fr"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archives-ouvertes.fr
  spf: true
hosts:
- cert_expires: Nov 22 00:00:17 2026 GMT
  host: www.ens-lyon.fr
  hsts: false
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
name: Ens Lyon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for École Normale Supérieure de Lyon, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: École Normale Supérieure de Lyon
provider_slug: ens-lyon
slug: ens-lyon-domain-security
source_filename: ens-lyon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ens-lyon.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 00:00:17 2026 GMT\n  hsts: false\n- host: api.archives-ouvertes.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ens-lyon.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: archives-ouvertes.fr\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 iodef \"mailto:ccsd-tech@ccsd.cnrs.fr\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ens-lyon/refs/heads/main/security/ens-lyon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- France
- Open Access
- Research
- Institutional Repository
- OAI-PMH
---
