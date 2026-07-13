---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: netskope.com
  spf: true
hosts:
- cert_expires: Nov  4 20:36:02 2026 GMT
  host: www.netskope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 17:11:13 2026 GMT
  host: docs.netskope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netskope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netskope, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Netskope
provider_slug: netskope
slug: netskope-domain-security
source_filename: netskope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netskope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 20:36:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.netskope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 17:11:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netskope.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netskope/refs/heads/main/security/netskope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- SASE
- SSE
- CASB
- Zero Trust
- SWG
- DLP
- Cloud Security
---
