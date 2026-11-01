---
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "pki.dfn.de"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gfz-potsdam.de
  spf: true
hosts:
- cert_expires: May 10 11:36:26 2027 GMT
  host: www.gfz-potsdam.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gfz Potsdam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GFZ Potsdam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GFZ Potsdam
provider_slug: gfz-potsdam
slug: gfz-potsdam-domain-security
source_filename: gfz-potsdam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gfz-potsdam.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 10 11:36:26 2027 GMT\n  hsts: false\ndomains:\n- domain: gfz-potsdam.de\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"pki.dfn.de\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gfz-potsdam/security/gfz-potsdam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geosciences
- Research
- Data
- EarthScience
---
