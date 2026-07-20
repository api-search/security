---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cdap.io
  spf: true
  spf_record: v=spf1 -all
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cask.co
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mktomail.com include:spf.mandrillapp.com ~all
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  note: third-party documentation host, not operated by Cask/CDAP
  spf: true
hosts:
- cert_expires: Oct 13 16:13:47 2026 GMT
  cert_subject: CN=cdap.io
  host: cdap.io
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:03:17 2023 GMT
  cert_subject: CN=docs.cdap.io
  host: docs.cdap.io
  hsts: false
  https: false
  https_error: certificate has expired
  note: 301 redirects to https://cdap.atlassian.net/wiki/spaces/DOCS/overview once the cert error is bypassed
  tls_version: TLSv1.3
- host: cask.co
  hsts: false
  http_status: 404
  https: false
  https_error: certificate name mismatch (CN=*.wpengine.com)
  note: company domain no longer serves Cask content
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: cdap.atlassian.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: third-party documentation host (Atlassian Confluence Cloud)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cask Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cask, probed live across 4 host(s) and 3 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cask
provider_slug: cask
slug: cask-domain-security
source_filename: cask-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the surviving Cask/CDAP hosts\nnotes: >-\n  Cask Data's own domain (cask.co) no longer serves the company site — it resolves to a WP Engine\n  parking host whose certificate is issued for *.wpengine.com and whose HTTP responses are 404.\n  The CDAP documentation host docs.cdap.io serves an expired certificate (expired 2023-09-27) and,\n  when the certificate error is bypassed, 301-redirects to the CDAP Confluence wiki. The living,\n  healthy host is cdap.io.\nhosts:\n- host: cdap.io\n  https: true\n  http_status: 200\n  tls_version: TLSv1.3\n  cert_subject: CN=cdap.io\n  cert_expires: Oct 13 16:13:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cdap.io\n  https: false\n  https_error: certificate has expired\n  tls_version: TLSv1.3\n  cert_subject: CN=docs.cdap.io\n  cert_expires: Sep 27 17:03:17 2023 GMT\n  hsts: false\n  note: 301 redirects to https://cdap.atlassian.net/wiki/spaces/DOCS/overview\
  \ once the cert error is bypassed\n- host: cask.co\n  https: false\n  https_error: certificate name mismatch (CN=*.wpengine.com)\n  http_status: 404\n  hsts: false\n  note: company domain no longer serves Cask content\n- host: cdap.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: third-party documentation host (Atlassian Confluence Cloud)\ndomains:\n- domain: cdap.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: true\n  dmarc_policy: reject\n- domain: cask.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:mktomail.com include:spf.mandrillapp.com ~all\n  dmarc: true\n  dmarc_policy: none\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: reject\n  note: third-party documentation host, not operated by Cask/CDAP\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cask/refs/heads/main/security/cask-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Big Data
- Data Analytics
- Data Pipelines
- Data Integration
- ETL
- Hadoop
- Spark
- Open Source
- CDAP
- Metadata
- Data Governance
- Acquired
---
