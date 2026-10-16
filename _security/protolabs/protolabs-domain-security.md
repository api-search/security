---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: protolabs.com
  spf: true
hosts:
- cert_expires: Nov 28 22:30:29 2026 GMT
  host: www.protolabs.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Protolabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protolabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Protolabs
provider_slug: protolabs
slug: protolabs-domain-security
source_filename: protolabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.protolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 22:30:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: protolabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protolabs/refs/heads/main/security/protolabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- RapidPrototyping
- DigitalManufacturing
- Engineering
---
