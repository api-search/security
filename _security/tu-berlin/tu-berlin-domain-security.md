---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tu.berlin
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tu-berlin.de
  spf: true
hosts:
- cert_expires: Dec 11 15:56:40 2026 GMT
  host: www.tu.berlin
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 10:49:30 2026 GMT
  host: depositonce.tu-berlin.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 10:49:56 2026 GMT
  host: api-depositonce.tu-berlin.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tu Berlin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technical University of Berlin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Technical University of Berlin
provider_slug: tu-berlin
slug: tu-berlin-domain-security
source_filename: tu-berlin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tu.berlin\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 15:56:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: depositonce.tu-berlin.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 10:49:30 2026 GMT\n  hsts: false\n- host: api-depositonce.tu-berlin.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 10:49:56 2026 GMT\n  hsts: false\ndomains:\n- domain: tu.berlin\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tu-berlin.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-berlin/refs/heads/main/security/tu-berlin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Repository
- Library
- Germany
---
