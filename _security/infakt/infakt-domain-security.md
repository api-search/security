---
description: ''
domains:
- caa:
  - 0 issuewild "elektronicznypodpis.pl"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:caa@infakt.pl"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: infakt.pl
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.infakt.pl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 15:38:40 2026 GMT
  host: docs.infakt.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.infakt.pl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infakt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for inFakt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: inFakt
provider_slug: infakt
slug: infakt-domain-security
source_filename: infakt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infakt.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.infakt.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:38:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.infakt.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: infakt.pl\n  dnssec: true\n  caa:\n  - 0 issuewild \"elektronicznypodpis.pl\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:caa@infakt.pl\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infakt/refs/heads/main/security/infakt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Accounting
- Invoicing
- Fintech
- Bookkeeping
- e-Invoicing
- KSeF
- Tax
- Poland
- SMB
---
