---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "quovadisglobal.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ciscospark.com
  spf: true
hosts:
- cert_expires: Nov 27 06:37:20 2026 GMT
  host: developer.ciscospark.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Spark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Spark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cisco Spark
provider_slug: cisco-spark
slug: cisco-spark-domain-security
source_filename: cisco-spark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ciscospark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 06:37:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ciscospark.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-spark/refs/heads/main/security/cisco-spark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social
- Public APIs
---
