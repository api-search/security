---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: buysight.com
  mx: []
  nameservers:
  - ns1.markmonitor.com
  - ns2.markmonitor.com
  - ns3.markmonitor.com
  - ns4.markmonitor.com
  - ns5.markmonitor.com
  - ns6.markmonitor.com
  - ns7.markmonitor.com
  spf: false
hosts:
- a_records:
  - 3.33.139.32
  host: buysight.com
  hsts: false
  http_final_url: http://comingsoon.markmonitor.com/
  http_status: 200
  https: false
  https_error: connection timed out (port 443 unreachable)
  tls_version: null
- host: www.buysight.com
  hsts: false
  https: false
  https_error: connection timed out (port 443 unreachable)
kind: domain-security
layout: security
method: probed
name: Buysight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buysight, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Buysight
provider_slug: buysight
slug: buysight-domain-security
source_filename: buysight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + openssl s_client + curl against buysight.com (2026-07-20)\nnote: >-\n  Buysight was acquired by AOL's Advertising.com Group on 2012-12-04 and no longer\n  operates. The buysight.com domain is registered through MarkMonitor (corporate\n  brand-protection registrar) and serves no live service. HTTPS does not answer;\n  plain HTTP redirects to the registrar placeholder at comingsoon.markmonitor.com.\n  Absence of records below is real probed data, not a gap in the probe.\nhosts:\n- host: buysight.com\n  https: false\n  https_error: connection timed out (port 443 unreachable)\n  http_status: 200\n  http_final_url: http://comingsoon.markmonitor.com/\n  tls_version: null\n  hsts: false\n  a_records:\n  - 3.33.139.32\n- host: www.buysight.com\n  https: false\n  https_error: connection timed out (port 443 unreachable)\n  hsts: false\ndomains:\n- domain: buysight.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy:\
  \ null\n  mx: []\n  nameservers:\n  - ns1.markmonitor.com\n  - ns2.markmonitor.com\n  - ns3.markmonitor.com\n  - ns4.markmonitor.com\n  - ns5.markmonitor.com\n  - ns6.markmonitor.com\n  - ns7.markmonitor.com\nwell_known:\n- path: /.well-known/security.txt\n  status: null\n  result: unreachable (no HTTPS listener)\n- path: /.well-known/openid-configuration\n  status: null\n  result: unreachable (no HTTPS listener)\n- path: /.well-known/api-catalog\n  status: null\n  result: unreachable (no HTTPS listener)\nregistries_checked:\n- registry: github-org\n  url: https://github.com/buysight\n  status: 404\n- registry: npm\n  query: buysight\n  result: no packages\n- registry: pypi\n  url: https://pypi.org/pypi/buysight/json\n  status: 404\narchived:\n  wayback_latest: http://web.archive.org/web/20121126034725/http://www.buysight.com:80/\n  wayback_timestamp: '20121126034725'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buysight/refs/heads/main/security/buysight-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Advertising
- Advertising Technology
- AdTech
- Retargeting
- Audience Targeting
- Dynamic Creative Optimization
- Marketing
- Machine Learning
- Acquired
- Defunct
---
