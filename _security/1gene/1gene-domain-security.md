---
description: TLS/HSTS/DNS posture for the registrable domain 1GENE actually controls. Probed by hand rather than by probe-domain-security.py, because that helper reads hosts from a Website or Portal pointer in apis.yml and 1GENE deliberately carries neither — its web origin currently serves an unconfigured placeholder (see well-known/1gene-well-known.yml). Absence of a record is valid data, not a failed probe.
domains: []
hosts:
- address: 121.199.172.246
  cert_expires: null
  host: www.1gene.com.cn
  hsts: false
  hsts_max_age: null
  http: true
  http_note: Plain HTTP returns the 1,033-byte Nginx Proxy Manager "Default Site" placeholder, Last-Modified 2026-06-03. No Strict-Transport-Security header is sent.
  http_status: 200
  https: false
  https_note: The origin accepts the TCP connection on 443 but aborts the TLS handshake with unrecognized_name (fatal alert 112) for SNI www.1gene.com.cn — no certificate is provisioned for the hostname. Observed with both LibreSSL 3.3.6 and OpenSSL.
  server: openresty
  tls_version: null
- address: 114.55.152.1
  host: 1gene.com.cn
  http: false
  https: false
  note: No response on 80 or 443; curl times out at 30s.
- address: 120.26.129.84
  host: mall.1gene.com.cn
  hsts: false
  http: true
  http_status: 404
  https: false
  https_note: Port 443 refuses the connection.
- address: 121.196.131.75
  host: m.1gene.com.cn
  http: false
  https: false
  note: No response on 80 or 443; curl times out.
- address: 121.199.69.226
  host: admin.1gene.com.cn
  http: false
  https: false
  note: No response on 80 or 443; curl times out.
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: 1Gene Domain Security
name_suffix: Domain Security
overview: Domain security posture for 1GENE, probed live across 5 host(s) and 0 registrable domain(s).
provider_name: 1GENE
provider_slug: 1gene
slug: 1gene-domain-security
source_filename: 1gene-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: 1gene.com.cn (dig + openssl s_client + curl, 2026-09-05)\nname: 1GENE domain security posture\ndescription: >-\n  TLS/HSTS/DNS posture for the registrable domain 1GENE actually controls. Probed by hand\n  rather than by probe-domain-security.py, because that helper reads hosts from a Website\n  or Portal pointer in apis.yml and 1GENE deliberately carries neither — its web origin\n  currently serves an unconfigured placeholder (see well-known/1gene-well-known.yml).\n  Absence of a record is valid data, not a failed probe.\n\nregistrable_domain: 1gene.com.cn\n\nregistration:\n  registrar: 阿里云计算有限公司（万网） / Alibaba Cloud (HiChina)\n  registrant_organization: 杭州尚壹生物科技有限公司 (Hangzhou Shangyi Biotechnology Co., Ltd.)\n  created: '2014-04-06'\n  expires: '2027-04-06'\n  status: ok\n  source: whois.cnnic.cn\n\nhosts:\n- host: www.1gene.com.cn\n  address: 121.199.172.246\n  https: false\n  https_note: >-\n    The origin accepts the TCP connection\
  \ on 443 but aborts the TLS handshake with\n    unrecognized_name (fatal alert 112) for SNI www.1gene.com.cn — no certificate is\n    provisioned for the hostname. Observed with both LibreSSL 3.3.6 and OpenSSL.\n  tls_version: null\n  cert_expires: null\n  http: true\n  http_status: 200\n  server: openresty\n  hsts: false\n  hsts_max_age: null\n  http_note: >-\n    Plain HTTP returns the 1,033-byte Nginx Proxy Manager \"Default Site\" placeholder,\n    Last-Modified 2026-06-03. No Strict-Transport-Security header is sent.\n- host: 1gene.com.cn\n  address: 114.55.152.1\n  https: false\n  http: false\n  note: No response on 80 or 443; curl times out at 30s.\n- host: mall.1gene.com.cn\n  address: 120.26.129.84\n  https: false\n  https_note: Port 443 refuses the connection.\n  http: true\n  http_status: 404\n  hsts: false\n- host: m.1gene.com.cn\n  address: 121.196.131.75\n  https: false\n  http: false\n  note: No response on 80 or 443; curl times out.\n- host: admin.1gene.com.cn\n  address:\
  \ 121.199.69.226\n  https: false\n  http: false\n  note: No response on 80 or 443; curl times out.\n\ndns:\n  dnssec: false\n  dnssec_evidence: 'dig DNSKEY 1gene.com.cn -> empty; dig DS 1gene.com.cn -> empty; whois DNSSEC: unsigned'\n  caa: []\n  caa_present: false\n  spf: v=spf1 include:spf.163.com -all\n  spf_present: true\n  dmarc: null\n  dmarc_present: false\n  dmarc_evidence: dig TXT _dmarc.1gene.com.cn -> empty\n  mx:\n  - 5 hzmx01.mxmail.netease.com\n  - 10 hzmx02.mxmail.netease.com\n  nameservers:\n  - dns31.hichina.com\n  - dns32.hichina.com\n\nsummary:\n  https_enforced: false\n  hsts: false\n  dnssec: false\n  caa: false\n  spf: true\n  dmarc: false\n  note: >-\n    Mail is configured with a strict SPF policy (-all) but no DMARC record, and the web\n    tier serves no HTTPS certificate at all. Nothing here is scored against the company's\n    API posture — there is no API — but it is the observable security surface of the\n    domain as of the probe date.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1gene/refs/heads/main/security/1gene-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Health
- Healthcare
- Biotechnology
- Genomics
- Diagnostics
- Cancer Screening
- Precision Medicine
- Life Sciences
- China
---
