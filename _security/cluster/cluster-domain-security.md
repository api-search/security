---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datacluster.com
  spf: true
hosts:
- cert_expires: Jan  5 10:43:40 2027 GMT
  host: datacluster.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cluster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cluster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cluster
provider_slug: cluster
slug: cluster-domain-security
source_filename: cluster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacluster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 10:43:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datacluster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cluster/refs/heads/main/security/cluster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- API
- eCommerce
- Product
---
