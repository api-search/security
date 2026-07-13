---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "certainly.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: frends.com
  spf: true
hosts:
- cert_expires: Oct  7 09:13:05 2026 GMT
  host: www.frends.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 13:46:40 2026 GMT
  host: docs.frends.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frends Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frends, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Frends
provider_slug: frends
slug: frends-domain-security
source_filename: frends-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frends.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:13:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.frends.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:46:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frends.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frends/refs/heads/main/security/frends-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration
- iPaaS
---
