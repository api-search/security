---
description: ''
domains:
- caa: []
  created: '2021-04-16'
  dmarc: false
  dnssec: false
  domain: liangzizhige.com
  mx: []
  registrar: Alibaba Cloud Computing (Beijing) Co., Ltd.
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: mailto:dmarc_report@service.aliyun.com
  dnssec: false
  domain: quantasing.com
  mx:
  - mx1.qiye.aliyun.com
  - mx2.qiye.aliyun.com
  - mx3.qiye.aliyun.com
  registrar: Alibaba Cloud Computing (Beijing) Co., Ltd.
  spf: true
  spf_record: v=spf1 include:spf1.dm.aliyun.com include:spf.qiye.aliyun.com -all
hosts:
- host: liangzizhige.com
  https: false
  note: no A record; domain registered via Alibaba Cloud, HiChina nameservers
  resolves: false
- host: www.liangzizhige.com
  https: false
  resolves: false
- host: ir.liangzizhige.com
  http_status: 301
  https: true
  redirects_to: https://ir.quantasing.com/
  resolves: true
- cert_issuer: C=US, O=Let's Encrypt, CN=YR2
  cert_not_after: '2026-09-25T14:49:45Z'
  cert_subject: CN=leapfrog-ssl-54.gcs-web.com
  host: ir.quantasing.com
  hsts: false
  http_status: 403
  http_version: HTTP/2
  https: true
  note: third-party investor-relations host (GCS-Web / Akamai), not company-operated
  resolves: true
  tls_version: TLSv1.3
- host: quantasing.com
  https: false
  note: no A record; mail-only domain (Alibaba Cloud corporate mail)
  resolves: false
kind: domain-security
layout: security
method: probed
name: Liangzizhige Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for liangzizhige, probed live across 5 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: liangzizhige
provider_slug: liangzizhige
slug: liangzizhige-domain-security
source_filename: liangzizhige-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes (dig @8.8.8.8, openssl s_client, curl) of the\n  apis.yml Website host and the company hosts discovered during enrichment\nnotes: >-\n  The corporate domain listed for this company (liangzizhige.com) is registered\n  but publishes no A record, so it serves no website and could not be probed over\n  HTTPS. The only live company host found is the investor-relations site, which\n  redirects to ir.quantasing.com and is fronted by Akamai/GCS-Web with bot\n  protection returning HTTP 403 to automated clients.\nhosts:\n- host: liangzizhige.com\n  https: false\n  resolves: false\n  note: no A record; domain registered via Alibaba Cloud, HiChina nameservers\n- host: www.liangzizhige.com\n  https: false\n  resolves: false\n- host: ir.liangzizhige.com\n  https: true\n  resolves: true\n  http_status: 301\n  redirects_to: https://ir.quantasing.com/\n- host: ir.quantasing.com\n  https: true\n  resolves: true\n  http_status:\
  \ 403\n  http_version: HTTP/2\n  tls_version: TLSv1.3\n  cert_issuer: \"C=US, O=Let's Encrypt, CN=YR2\"\n  cert_subject: CN=leapfrog-ssl-54.gcs-web.com\n  cert_not_after: '2026-09-25T14:49:45Z'\n  hsts: false\n  note: third-party investor-relations host (GCS-Web / Akamai), not company-operated\n- host: quantasing.com\n  https: false\n  resolves: false\n  note: no A record; mail-only domain (Alibaba Cloud corporate mail)\ndomains:\n- domain: liangzizhige.com\n  registrar: Alibaba Cloud Computing (Beijing) Co., Ltd.\n  created: '2021-04-16'\n  dnssec: false\n  caa: []\n  mx: []\n  spf: false\n  dmarc: false\n- domain: quantasing.com\n  registrar: Alibaba Cloud Computing (Beijing) Co., Ltd.\n  dnssec: false\n  caa: []\n  mx:\n  - mx1.qiye.aliyun.com\n  - mx2.qiye.aliyun.com\n  - mx3.qiye.aliyun.com\n  spf: true\n  spf_record: v=spf1 include:spf1.dm.aliyun.com include:spf.qiye.aliyun.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_rua: mailto:dmarc_report@service.aliyun.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liangzizhige/refs/heads/main/security/liangzizhige-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Online Learning
- Consumer
- Personal Finance
- China
- Venture Backed
---
