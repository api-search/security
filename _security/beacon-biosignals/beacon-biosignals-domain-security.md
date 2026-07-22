---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beacon.bio
  spf: true
hosts:
- cert_expires: Sep 22 01:56:38 2026 GMT
  host: beacon.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beacon Biosignals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beacon Biosignals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beacon Biosignals
provider_slug: beacon-biosignals
slug: beacon-biosignals-domain-security
source_filename: beacon-biosignals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beacon.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:56:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beacon.bio\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-biosignals/refs/heads/main/security/beacon-biosignals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Neurotechnology
- EEG
- Sleep
- Clinical Trials
- Brain Health
- Machine Learning
- Open Source
---
