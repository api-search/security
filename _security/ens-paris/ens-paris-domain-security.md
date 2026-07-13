---
api_specs:
- filename: ens-paris-mesr-opendata.yaml
  format: yaml
  label: MESR Higher Education Open Data (Explore API)
  slug: mesr-opendata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ens-paris/refs/heads/main/openapi/ens-paris-mesr-opendata.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "harica.gr"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: psl.eu
  spf: true
- caa:
  - 0 issue "harica.gr"
  - 0 iodef "mailto:ccsd-tech@ccsd.cnrs.fr"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archives-ouvertes.fr
  spf: true
hosts:
- cert_expires: Oct  9 13:05:10 2026 GMT
  host: www.ens.psl.eu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 12:16:58 2026 GMT
  host: api.archives-ouvertes.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 12:15:53 2026 GMT
  host: api.hal.science
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ens Paris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for École Normale Supérieure de Paris, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: École Normale Supérieure de Paris
provider_slug: ens-paris
slug: ens-paris-domain-security
source_filename: ens-paris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ens.psl.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:05:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.archives-ouvertes.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hal.science\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:15:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: psl.eu\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: archives-ouvertes.fr\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:ccsd-tech@ccsd.cnrs.fr\"\n  - 0 issuewild\
  \ \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ens-paris/refs/heads/main/security/ens-paris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Open Access
- France
---
