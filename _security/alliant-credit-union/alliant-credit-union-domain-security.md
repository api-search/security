---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alliantcreditunion.org
  spf: true
hosts:
- cert_expires: Oct 19 17:02:53 2026 GMT
  host: www.alliantcreditunion.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Alliant Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alliant Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alliant Credit Union
provider_slug: alliant-credit-union
slug: alliant-credit-union-domain-security
source_filename: alliant-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alliantcreditunion.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 17:02:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: alliantcreditunion.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliant-credit-union/refs/heads/main/security/alliant-credit-union-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Credit Union
- Open Finance
- Data Aggregation
- Consumer Banking
---
