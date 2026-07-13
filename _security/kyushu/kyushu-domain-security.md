---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Kyushu University Institutional Repository (QIR) OAI-PMH
  slug: qir-oai-pmh
  spec_type: OpenAPI
  url: https://catalog.lib.kyushu-u.ac.jp/mmd/mmd_api/oai-pmh/?verb=Identify
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kyushu-u.ac.jp
  spf: true
hosts:
- cert_expires: Mar 12 23:18:16 2027 GMT
  host: www.kyushu-u.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 19 05:08:25 2027 GMT
  host: www.lib.kyushu-u.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 02:33:05 2027 GMT
  host: catalog.lib.kyushu-u.ac.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kyushu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyushu University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kyushu University
provider_slug: kyushu
slug: kyushu-domain-security
source_filename: kyushu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kyushu-u.ac.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 12 23:18:16 2027 GMT\n  hsts: false\n- host: www.lib.kyushu-u.ac.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 05:08:25 2027 GMT\n  hsts: false\n- host: catalog.lib.kyushu-u.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 02:33:05 2027 GMT\n  hsts: null\ndomains:\n- domain: kyushu-u.ac.jp\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyushu/refs/heads/main/security/kyushu-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Institutional Repository
- OAI-PMH
- Open Access
- Japan
---
