---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "e5.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hhs.gov
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acf.gov
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.acf.hhs.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 20:21:05 2026 GMT
  host: tanfdata.acf.hhs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: acf.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: The Administration For Children And Families Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Administration for Children and Families, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Administration for Children and Families
provider_slug: the-administration-for-children-and-families
slug: the-administration-for-children-and-families-domain-security
source_filename: the-administration-for-children-and-families-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acf.hhs.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: tanfdata.acf.hhs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:21:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: acf.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hhs.gov\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"e5.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: acf.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-administration-for-children-and-families/refs/heads/main/security/the-administration-for-children-and-families-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Children
- Families
- Federal Government
- Health And Human Services
- Human Services
- Social Safety Net
---
