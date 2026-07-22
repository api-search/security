---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "26caf1396a7087273d5c93611d7908f5.bd0506eac4b9c2bb6acb66fdabaf5202.sectigo.com"
  - 0 issue "pki.goog"
  - 0 issuemail "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gov2x.com
  spf: true
hosts:
- cert_expires: Aug 17 12:41:38 2026 GMT
  host: www.gov2x.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: V2X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for V2X, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: V2X
provider_slug: v2x
slug: v2x-domain-security
source_filename: v2x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gov2x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 12:41:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: gov2x.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"26caf1396a7087273d5c93611d7908f5.bd0506eac4b9c2bb6acb66fdabaf5202.sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuemail \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/v2x/refs/heads/main/security/v2x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Defense
- National Security
- Government Services
- Aerospace
- Cybersecurity
---
