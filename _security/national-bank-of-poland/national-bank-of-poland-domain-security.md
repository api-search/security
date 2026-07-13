---
description: ''
domains:
- caa:
  - 0 issue "certum.pl"
  - 0 issueewild "certum.pl"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nbp.pl
  spf: true
hosts:
- cert_expires: Sep 24 12:56:39 2026 GMT
  host: api.nbp.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Bank Of Poland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Bank of Poland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Bank of Poland
provider_slug: national-bank-of-poland
slug: national-bank-of-poland-domain-security
source_filename: national-bank-of-poland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nbp.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:56:39 2026 GMT\n  hsts: false\ndomains:\n- domain: nbp.pl\n  dnssec: false\n  caa:\n  - 0 issue \"certum.pl\"\n  - 0 issueewild \"certum.pl\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-bank-of-poland/refs/heads/main/security/national-bank-of-poland-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency Exchange
- Public APIs
---
