---
description: ''
domains:
- caa:
  - 128 iodef "mailto:securite@bforbank.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bforbank.com
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: www.bforbank.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bforbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bforbank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bforbank
provider_slug: bforbank
slug: bforbank-domain-security
source_filename: bforbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bforbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bforbank.com\n  dnssec: true\n  caa:\n  - 128 iodef \"mailto:securite@bforbank.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bforbank/refs/heads/main/security/bforbank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Banking
- Digital Bank
- France
- Fintech
---
