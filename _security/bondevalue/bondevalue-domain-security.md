---
description: ''
domains:
- caa:
  - 0 issue "starfieldtech.com"
  - 0 issue "godaddy.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bondblox.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: bondblox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bondevalue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bondevalue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bondevalue
provider_slug: bondevalue
slug: bondevalue-domain-security
source_filename: bondevalue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bondblox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bondblox.com\n  dnssec: true\n  caa:\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bondevalue/refs/heads/main/security/bondevalue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- FinTech
- Bonds
- Investment
- Platform
- Singapore
---
