---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "buypass.com"
  - 0 iodef "mailto:security@kartverket.no"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kartverket.no
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.kartverket.no
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Statens Kartverk Norwegian Mapping Authority Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statens kartverk - Norwegian Mapping Authority, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Statens kartverk - Norwegian Mapping Authority
provider_slug: statens-kartverk-norwegian-mapping-authority
slug: statens-kartverk-norwegian-mapping-authority-domain-security
source_filename: statens-kartverk-norwegian-mapping-authority-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kartverket.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kartverket.no\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"buypass.com\"\n  - 0 iodef \"mailto:security@kartverket.no\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/statens-kartverk-norwegian-mapping-authority/security/statens-kartverk-norwegian-mapping-authority-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
