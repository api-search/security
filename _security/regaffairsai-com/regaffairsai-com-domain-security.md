---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: regaffairsai.com
  spf: true
hosts:
- cert_expires: Feb  2 20:25:38 2027 GMT
  host: regaffairsai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RegAffairs AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RegAffairs AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RegAffairs AI
provider_slug: regaffairsai-com
slug: regaffairsai-com-domain-security
source_filename: regaffairsai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regaffairsai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 20:25:38 2027 GMT\n  hsts: false\ndomains:\n- domain: regaffairsai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/regaffairsai-com/security/regaffairsai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Regulatory
- Data
- Compliance
- Healthcare
---
