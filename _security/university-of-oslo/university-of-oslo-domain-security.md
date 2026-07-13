---
description: ''
domains:
- caa:
  - 0 issuewild "harica.gr"
  - 0 issue "harica.gr"
  - 0 iodef "mailto:cert@uio.no"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uio.no
  spf: true
hosts:
- cert_expires: Dec  5 16:56:48 2026 GMT
  host: data.uio.no
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Oslo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Oslo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Oslo
provider_slug: university-of-oslo
slug: university-of-oslo-domain-security
source_filename: university-of-oslo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.uio.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 16:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: uio.no\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:cert@uio.no\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-oslo/refs/heads/main/security/university-of-oslo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- Public APIs
---
