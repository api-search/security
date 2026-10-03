---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bondbloxxetf.com
  spf: true
hosts:
- cert_expires: Nov  5 00:09:19 2026 GMT
  host: bondbloxxetf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bondbloxx Investment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bondbloxx Investment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bondbloxx Investment
provider_slug: bondbloxx-investment
slug: bondbloxx-investment-domain-security
source_filename: bondbloxx-investment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bondbloxxetf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 00:09:19 2026 GMT\n  hsts: false\ndomains:\n- domain: bondbloxxetf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bondbloxx-investment/refs/heads/main/security/bondbloxx-investment-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- ETFs
- Fixed Income
- Investment
- Asset Management
---
