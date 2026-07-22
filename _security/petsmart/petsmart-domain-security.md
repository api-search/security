---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 iodef "mailto:pmcaa@petsmart.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: petsmart.com
  spf: true
hosts:
- cert_expires: Sep 27 18:18:00 2026 GMT
  host: www.petsmart.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Petsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PetSmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PetSmart
provider_slug: petsmart
slug: petsmart-domain-security
source_filename: petsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.petsmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:18:00 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: petsmart.com\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:pmcaa@petsmart.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petsmart/refs/heads/main/security/petsmart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Pets
- Fortune 1000
---
