---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beginlearning.com
  spf: true
hosts:
- cert_expires: Dec 20 22:58:32 2026 GMT
  host: www.beginlearning.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beginlearning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beginlearning, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beginlearning
provider_slug: beginlearning
slug: beginlearning-domain-security
source_filename: beginlearning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beginlearning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 22:58:32 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: beginlearning.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beginlearning/refs/heads/main/security/beginlearning-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Children
- Learning
- DigitalApps
- Toys
---
