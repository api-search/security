---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perspectiveapi.com
  spf: true
hosts:
- cert_expires: Aug 22 02:10:00 2026 GMT
  host: perspectiveapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perspective Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perspective, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perspective
provider_slug: perspective
slug: perspective-domain-security
source_filename: perspective-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perspectiveapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:10:00 2026 GMT\n  hsts: false\ndomains:\n- domain: perspectiveapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perspective/refs/heads/main/security/perspective-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Machine Learning
- Public APIs
---
