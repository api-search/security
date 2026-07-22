---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pydata.org
  spf: true
hosts:
- cert_expires: Sep 23 01:30:26 2026 GMT
  host: pandas.pydata.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pandas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pandas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: pandas
provider_slug: pandas
slug: pandas-domain-security
source_filename: pandas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pandas.pydata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:30:26 2026 GMT\n  hsts: false\ndomains:\n- domain: pydata.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandas/refs/heads/main/security/pandas-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Analysis
- Data Science
- Library
- Open Source
- Python
---
