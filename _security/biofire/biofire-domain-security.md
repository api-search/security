---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: biofire.com
  spf: true
hosts:
- cert_expires: Oct 28 17:04:02 2026 GMT
  host: biofire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biofire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biofire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Biofire
provider_slug: biofire
slug: biofire-domain-security
source_filename: biofire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biofire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:04:02 2026 GMT\n  hsts: false\ndomains:\n- domain: biofire.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biofire/refs/heads/main/security/biofire-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Heating
- Ceramics
- CustomDesign
- GermanManufacturing
---
