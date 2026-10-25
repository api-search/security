---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:licensing@nsrltd.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nsrltd.com
  spf: true
hosts:
- cert_expires: Dec 26 19:31:28 2026 GMT
  host: nsrltd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Northern Star Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northern Star Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Northern Star Resources
provider_slug: northern-star-resources
slug: northern-star-resources-domain-security
source_filename: northern-star-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nsrltd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 19:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nsrltd.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:licensing@nsrltd.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northern-star-resources/refs/heads/main/security/northern-star-resources-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Gold
- Australia
- Natural Resources
- ASX Listed
---
