---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sparkcarwash.com
  spf: true
hosts:
- cert_expires: Nov 23 01:43:27 2026 GMT
  host: sparkcarwash.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spark Car Wash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spark Car Wash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spark Car Wash
provider_slug: spark-car-wash
slug: spark-car-wash-domain-security
source_filename: spark-car-wash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sparkcarwash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 01:43:27 2026 GMT\n  hsts: false\ndomains:\n- domain: sparkcarwash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-car-wash/refs/heads/main/security/spark-car-wash-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Car Wash
- Automotive Services
- Consumer Services
- Retail
- Subscriptions
- Memberships
- New Jersey
- United States
---
