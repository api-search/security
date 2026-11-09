---
description: ''
domains:
- caa:
  - 0 iodef "mailto:abuse@avinor.no"
  - 0 issuewild "www.digicert.com"
  - 0 issue "www.digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: avinor.no
  spf: true
hosts:
- cert_expires: Jan 26 12:42:46 2027 GMT
  host: avinor.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avinor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avinor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Avinor
provider_slug: avinor
slug: avinor-domain-security
source_filename: avinor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avinor.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 12:42:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avinor.no\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:abuse@avinor.no\"\n  - 0 issuewild \"www.digicert.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/avinor/security/avinor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Aviation
- Airport
- Norway
- Transportation
- Infrastructure
- Company
---
