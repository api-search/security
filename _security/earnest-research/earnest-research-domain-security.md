---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: earnestresearch.com
  spf: true
hosts:
- cert_expires: Jan  4 18:28:17 2027 GMT
  host: earnestresearch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earnest Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earnest Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Earnest Research
provider_slug: earnest-research
slug: earnest-research-domain-security
source_filename: earnest-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earnestresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 18:28:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: earnestresearch.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/earnest-research/security/earnest-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Data
- Analytics
- APIs
---
