---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atomicainformatics.com
  spf: true
hosts:
- cert_expires: Oct 13 00:37:40 2026 GMT
  host: atomicainformatics.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atomica Informatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomica Informatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Atomica Informatics
provider_slug: atomica-informatics
slug: atomica-informatics-domain-security
source_filename: atomica-informatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomicainformatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 00:37:40 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: atomicainformatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomica-informatics/refs/heads/main/security/atomica-informatics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Healthcare
- Health Informatics
- Clinical Data
- openEHR
- Interoperability
- Data Modeling
- Consulting
- Training
---
