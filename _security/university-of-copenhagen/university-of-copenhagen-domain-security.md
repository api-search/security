---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 issue "sectigo.com"
  - 0 issuewild "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ku.dk
  spf: true
hosts:
- cert_expires: Sep  5 23:23:34 2026 GMT
  host: www.ku.dk
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 15:28:44 2026 GMT
  host: researchprofiles.ku.dk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Copenhagen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Copenhagen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: University of Copenhagen
provider_slug: university-of-copenhagen
slug: university-of-copenhagen-domain-security
source_filename: university-of-copenhagen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ku.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:23:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: researchprofiles.ku.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:28:44 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: ku.dk\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-copenhagen/refs/heads/main/security/university-of-copenhagen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Denmark
- Nordic
- Open Source
---
