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
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "entrust.net"
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
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: acf.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 18 19:11:52 2026 GMT
  host: catalog.data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Administration For Native Americans Ana  Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Administration for Native Americans (ANA), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Administration for Native Americans (ANA)
provider_slug: administration-for-native-americans-ana-
slug: administration-for-native-americans-ana--domain-security
source_filename: administration-for-native-americans-ana--domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acf.hhs.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: acf.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: catalog.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:11:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hhs.gov\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"e5.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: acf.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/administration-for-native-americans-ana-/refs/heads/main/security/administration-for-native-americans-ana--domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Indigenous
- Native Americans
- Grants
- Social Services
- Language Preservation
- Open Data
---
