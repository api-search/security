---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ulb.be
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ulb.ac.be
  spf: true
hosts:
- cert_expires: Nov 26 10:06:41 2026 GMT
  host: www.ulb.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 10:06:41 2026 GMT
  host: bib.ulb.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 10:22:36 2026 GMT
  host: difusion-svc.ulb.ac.be
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ulb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Université libre de Bruxelles, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Université libre de Bruxelles
provider_slug: ulb
slug: ulb-domain-security
source_filename: ulb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ulb.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 10:06:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bib.ulb.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 10:06:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: difusion-svc.ulb.ac.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 10:22:36 2026 GMT\n  hsts: null\ndomains:\n- domain: ulb.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ulb.ac.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ulb/refs/heads/main/security/ulb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- Belgium
---
