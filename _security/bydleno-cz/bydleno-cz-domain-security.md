---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:klapuchdominik@gmail.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bydleno.cz
  spf: true
hosts:
- cert_expires: Jan 22 16:04:44 2027 GMT
  host: bydleno.cz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bydleno Cz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BDLN Data s.r.o., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BDLN Data s.r.o.
provider_slug: bydleno-cz
slug: bydleno-cz-domain-security
source_filename: bydleno-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bydleno.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 16:04:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bydleno.cz\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:klapuchdominik@gmail.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bydleno-cz/security/bydleno-cz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Rentals
- Czech Republic
- Data Aggregation
---
