---
api_specs:
- filename: swagger.json
  format: json
  label: Coscine Research Data API
  slug: coscine
  spec_type: OpenAPI
  url: https://coscine.rwth-aachen.de/coscine/api/swagger/v2/swagger.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:ca@rwth-aachen.de"
  - 0 issuemail "harica.gr"
  - 0 issue "harica.gr"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rwth-aachen.de
  spf: true
- caa:
  - 0 iodef "mailto:ca@rwth-aachen.de"
  - 0 issue "letsencrypt.org"
  - 0 issuemail "harica.gr"
  - 0 issue "harica.gr"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coscine.de
  spf: true
hosts:
- cert_expires: Oct  9 03:50:57 2026 GMT
  host: www.rwth-aachen.de
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 20 05:37:42 2026 GMT
  host: docs.coscine.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 14:03:10 2026 GMT
  host: coscine.rwth-aachen.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rwth Aachen University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RWTH Aachen University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RWTH Aachen University
provider_slug: rwth-aachen-university
slug: rwth-aachen-university-domain-security
source_filename: rwth-aachen-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rwth-aachen.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 03:50:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: docs.coscine.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:37:42 2026 GMT\n  hsts: false\n- host: coscine.rwth-aachen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 14:03:10 2026 GMT\n  hsts: false\ndomains:\n- domain: rwth-aachen.de\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:ca@rwth-aachen.de\"\n  - 0 issuemail \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: coscine.de\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:ca@rwth-aachen.de\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuemail \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rwth-aachen-university/refs/heads/main/security/rwth-aachen-university-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Germany
---
