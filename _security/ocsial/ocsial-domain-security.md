---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ocsial.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: tuball.com
  spf: true
  spf_policy: ?all
hosts:
- cert_expires: Nov 15 05:14:36 2026 GMT
  host: ocsial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 10:48:47 2026 GMT
  cert_issuer: Let's Encrypt
  host: tuball.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ocsial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OCSiAl, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OCSiAl
provider_slug: ocsial
slug: ocsial-domain-security
source_filename: ocsial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ocsial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 05:14:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tuball.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 10:48:47 2026 GMT\n  cert_issuer: Let's Encrypt\n  hsts: false\n  hsts_max_age: null\ndomains:\n- domain: ocsial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tuball.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: ?all\n  dmarc: false\n  dmarc_policy: null\nnote: 'Two company hosts probed: ocsial.com (corporate site) and tuball.com (TUBALL\n  product site). ocsial.com enforces HSTS (max-age 31536000, includeSubDomains) and\n  publishes DMARC p=reject via EasyDMARC; tuball.com serves no HSTS header, no DMARC\n  record and a soft-fail SPF (?all). Neither domain publishes DNSSEC or CAA records.\n\
  \  Absence of a record is recorded as measured, not inferred.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocsial/refs/heads/main/security/ocsial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advanced Materials
- Nanotechnology
- Carbon Nanotubes
- Chemicals
- Manufacturing
- Batteries
- Coatings
- Luxembourg
---
