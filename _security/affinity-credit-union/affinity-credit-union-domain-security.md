---
description: ''
domains:
- caa:
  - 0 issue "pki.goog;cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: affinitycu.ca
  spf: true
hosts:
- cert_expires: Mar 16 19:37:14 2027 GMT
  host: www.affinitycu.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affinity Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affinity Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Affinity Credit Union
provider_slug: affinity-credit-union
slug: affinity-credit-union-domain-security
source_filename: affinity-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.affinitycu.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 19:37:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: affinitycu.ca\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog;cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinity-credit-union/refs/heads/main/security/affinity-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Canada
- Credit Union
- Cooperative
- Saskatchewan
- Consumer-Driven Banking
- Open Banking
- Data Aggregation
---
