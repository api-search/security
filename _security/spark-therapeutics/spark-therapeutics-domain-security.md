---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gene.com
  spf: true
hosts:
- cert_expires: Sep 19 23:46:37 2026 GMT
  host: www.gene.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spark Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for spark-therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: spark-therapeutics
provider_slug: spark-therapeutics
slug: spark-therapeutics-domain-security
source_filename: spark-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: gene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-therapeutics/refs/heads/main/security/spark-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Pharmaceuticals
- Gene Therapy
- Rare Disease
- Ophthalmology
- Inherited Retinal Disease
- Roche Subsidiary
- Life Sciences
---
