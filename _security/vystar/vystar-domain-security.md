---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vystarcu.org
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.vystarcu.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vystar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VyStar Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VyStar Credit Union
provider_slug: vystar
slug: vystar-domain-security
source_filename: vystar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vystarcu.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: vystarcu.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vystar/refs/heads/main/security/vystar-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Financial Services
- Banking
- Credit Union
- United States
- Open Finance
- Consumer Finance
- Data Aggregation
---
