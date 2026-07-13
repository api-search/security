---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: roboflow.com
  spf: true
hosts:
- cert_expires: Sep 15 07:02:39 2026 GMT
  host: universe.roboflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roboflow Universe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roboflow Universe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Roboflow Universe
provider_slug: roboflow-universe
slug: roboflow-universe-domain-security
source_filename: roboflow-universe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: universe.roboflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:02:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: roboflow.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roboflow-universe/refs/heads/main/security/roboflow-universe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Machine Learning
- Public APIs
---
