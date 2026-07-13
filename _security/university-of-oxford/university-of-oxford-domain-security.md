---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ox.ac.uk
  spf: true
hosts:
- cert_expires: Sep 15 19:58:48 2026 GMT
  host: www.ox.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 00:58:37 2026 GMT
  host: ora.ox.ac.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Oxford Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Oxford, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Oxford
provider_slug: university-of-oxford
slug: university-of-oxford-domain-security
source_filename: university-of-oxford-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ox.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:58:48 2026 GMT\n  hsts: null\n- host: ora.ox.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:58:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: ox.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/security/university-of-oxford-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United Kingdom
- Open Access
- OAI-PMH
- Repository
---
