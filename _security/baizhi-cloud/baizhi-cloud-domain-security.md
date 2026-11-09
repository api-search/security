---
description: ''
domains:
- caa:
  - lb-6hkxeptz-mno4d5prgt37w82k.clb.sh-tencentclb.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: baizhi.cloud
  spf: false
hosts:
- cert_expires: Jan 18 16:31:51 2027 GMT
  host: baizhi.cloud
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Baizhi Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 长亭百智云, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: 长亭百智云
provider_slug: baizhi-cloud
slug: baizhi-cloud-domain-security
source_filename: baizhi-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baizhi.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 16:31:51 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: baizhi.cloud\n  dnssec: true\n  caa:\n  - lb-6hkxeptz-mno4d5prgt37w82k.clb.sh-tencentclb.com.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/baizhi-cloud/security/baizhi-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Cloud
- Platform
- Enterprise
- Chinese
---
