---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forkliftservicingcost.co.uk
  spf: true
hosts:
- cert_expires: Jan 10 00:59:05 2027 GMT
  host: forkliftservicingcost.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Forklift Servicing Cost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forklift Servicing Cost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forklift Servicing Cost
provider_slug: forkliftservicingcost-co-uk
slug: forkliftservicingcost-co-uk-domain-security
source_filename: forkliftservicingcost-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forkliftservicingcost.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 00:59:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: forkliftservicingcost.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/forkliftservicingcost-co-uk/security/forkliftservicingcost-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Forklift
- Servicing
- LOLER
- HSE
---
