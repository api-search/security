---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: seedandspark.com
  spf: true
hosts:
- cert_expires: Oct  9 23:16:16 2026 GMT
  host: seedandspark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seed And Spark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seed&Spark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Seed&Spark
provider_slug: seed-and-spark
slug: seed-and-spark-domain-security
source_filename: seed-and-spark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seedandspark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:16:16 2026 GMT\n  hsts: null\ndomains:\n- domain: seedandspark.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seed-and-spark/refs/heads/main/security/seed-and-spark-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crowdfunding
- Film
- Streaming
- Entertainment
- Media
- Independent Film
---
