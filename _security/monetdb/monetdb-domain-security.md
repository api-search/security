---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monetdb.org
  spf: true
hosts:
- cert_expires: Jan 14 18:18:59 2027 GMT
  host: monetdb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MonetDB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MonetDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MonetDB
provider_slug: monetdb
slug: monetdb-domain-security
source_filename: monetdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monetdb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 18:18:59 2027 GMT\n  hsts: false\ndomains:\n- domain: monetdb.org\n  dnssec: true\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/monetdb/security/monetdb-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Database
- Open Source
- Analytics
- SQL
- High Performance
---
