---
api_specs:
- filename: aarhus-pure-rest.yaml
  format: yaml
  label: Pure Research Portal Web Service (REST)
  slug: pure-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarhus/refs/heads/main/openapi/aarhus-pure-rest.yaml
description: ''
domains:
- caa:
  - 0 iodef "mailto:cert@au.dk"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: au.dk
  spf: true
hosts:
- cert_expires: Sep 23 06:47:30 2026 GMT
  host: www.au.dk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 18:15:25 2026 GMT
  host: pure.au.dk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:25:41 2026 GMT
  host: kursuskatalog.au.dk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aarhus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aarhus University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aarhus University
provider_slug: aarhus
slug: aarhus-domain-security
source_filename: aarhus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.au.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:47:30 2026 GMT\n  hsts: false\n- host: pure.au.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:15:25 2026 GMT\n  hsts: false\n- host: kursuskatalog.au.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:25:41 2026 GMT\n  hsts: false\ndomains:\n- domain: au.dk\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:cert@au.dk\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aarhus/refs/heads/main/security/aarhus-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Denmark
- Europe
---
