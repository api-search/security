---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brainkb.org
  spf: false
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: brainkb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainkb Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrainKB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BrainKB
provider_slug: brainkb-org
slug: brainkb-org-domain-security
source_filename: brainkb-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainkb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: brainkb.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/brainkb-org/security/brainkb-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Brain
- Neuroscience
- Data
- Research
- Platform
---
