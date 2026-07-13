---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "e5.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hhs.gov
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: npiregistry.cms.hhs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nppes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NPPES, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NPPES
provider_slug: nppes
slug: nppes-domain-security
source_filename: nppes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: npiregistry.cms.hhs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hhs.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"e5.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nppes/refs/heads/main/security/nppes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health
- Public APIs
---
