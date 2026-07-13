---
description: ''
domains:
- caa:
  - 0 issuewild "www.digicert.com"
  - 0 iodef "mailto:entsec-caa-monitoring@databricks.com"
  - 0 issue "1and1.digitalcertvalidation.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: databricks.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lakehouse Architecture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lakehouse Architecture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lakehouse Architecture
provider_slug: lakehouse-architecture
slug: lakehouse-architecture-domain-security
source_filename: lakehouse-architecture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: databricks.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"www.digicert.com\"\n  - 0 iodef \"mailto:entsec-caa-monitoring@databricks.com\"\n  - 0 issue \"1and1.digitalcertvalidation.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakehouse-architecture/refs/heads/main/security/lakehouse-architecture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Big Data
- Data Architecture
- Data Lake
- Data Warehouse
---
