---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digitalml.com
  spf: true
hosts:
- cert_expires: Dec 22 03:41:32 2026 GMT
  host: digitalml.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digitalml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigitalML, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DigitalML
provider_slug: digitalml
slug: digitalml-domain-security
source_filename: digitalml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitalml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 03:41:32 2026 GMT\n  hsts: false\ndomains:\n- domain: digitalml.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/digitalml/security/digitalml-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- Platform
- Enterprise
- DigitalTransformation
---
