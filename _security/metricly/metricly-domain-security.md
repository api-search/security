---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metricly.com
  spf: true
hosts:
- cert_expires: May 10 01:33:36 2027 GMT
  host: www.metricly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metricly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metricly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Metricly
provider_slug: metricly
slug: metricly-domain-security
source_filename: metricly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metricly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 10 01:33:36 2027 GMT\n  hsts: false\ndomains:\n- domain: metricly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/metricly/security/metricly-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
