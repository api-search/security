---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "harica.gr"
  - 0 issuewild "pki.dfn.de"
  - 0 iodef "mailto:pki@geomar.de"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geomar.de
  spf: true
hosts:
- cert_expires: Nov 24 17:23:35 2026 GMT
  host: www.geomar.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geomar Helmholtz Centre For Ocean Research Kiel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GEOMAR Helmholtz Centre for Ocean Research Kiel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GEOMAR Helmholtz Centre for Ocean Research Kiel
provider_slug: geomar-helmholtz-centre-for-ocean-research-kiel
slug: geomar-helmholtz-centre-for-ocean-research-kiel-domain-security
source_filename: geomar-helmholtz-centre-for-ocean-research-kiel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geomar.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 17:23:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: geomar.de\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"pki.dfn.de\"\n  - 0 iodef \"mailto:pki@geomar.de\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/geomar-helmholtz-centre-for-ocean-research-kiel/security/geomar-helmholtz-centre-for-ocean-research-kiel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Research
- Oceanography
- Climate
- MarineTechnology
---
