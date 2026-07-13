---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fbi.gov
  spf: true
hosts:
- cert_expires: Oct  8 01:34:31 2026 GMT
  host: www.fbi.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fbi Wanted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FBI Wanted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FBI Wanted
provider_slug: fbi-wanted
slug: fbi-wanted-domain-security
source_filename: fbi-wanted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fbi.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fbi.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fbi-wanted/refs/heads/main/security/fbi-wanted-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
