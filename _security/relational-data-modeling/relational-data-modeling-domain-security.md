---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikipedia.org
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:internalsecurity@sqldbm.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sqldbm.com
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikipedia.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 00:16:02 2026 GMT
  host: sqldbm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: hackolade.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relational Data Modeling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relational Data Modeling, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relational Data Modeling
provider_slug: relational-data-modeling
slug: relational-data-modeling-domain-security
source_filename: relational-data-modeling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: sqldbm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:16:02 2026 GMT\n  hsts: false\n- host: hackolade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sqldbm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild\
  \ \"sectigo.com\"\n  - 0 iodef \"mailto:internalsecurity@sqldbm.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relational-data-modeling/refs/heads/main/security/relational-data-modeling-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Architecture
- Database Design
- Entity Relationship
- Normalization
- SQL
- Schema Design
- Data Modeling
---
