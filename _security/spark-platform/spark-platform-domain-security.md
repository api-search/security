---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sparkapi.io
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sparkplatform.com
  spf: true
hosts:
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: www.sparkapi.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: sparkplatform.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: sparkapi.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 23:59:59 2026 GMT
  cert_issuer: ZeroSSL RSA DV SSL CA 2
  host: replication.sparkapi.com
  hsts: false
  https: true
  note: Added by hand on 2026-07-26 — the RESO Web API / replication host from apis.yml baseURL, which the automated pass did not resolve to a bare hostname. No Strict-Transport-Security header was returned on either the 301 at / or the 401 at /Version/3/Reso/OData/Property.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spark Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spark Platform, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spark Platform
provider_slug: spark-platform
slug: spark-platform-domain-security
source_filename: spark-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sparkapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: sparkplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: sparkapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: replication.sparkapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  cert_issuer: ZeroSSL RSA DV SSL CA 2\n  hsts: false\n  note: >-\n    Added by hand on 2026-07-26 — the RESO Web API / replication host from apis.yml baseURL,\n    which the automated pass did not resolve to a bare hostname. No\n    Strict-Transport-Security header was returned on either the 301 at / or the 401 at\n    /Version/3/Reso/OData/Property.\n\
  domains:\n- domain: sparkapi.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: sparkplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-platform/refs/heads/main/security/spark-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- Listing Data Infrastructure
- OData
---
