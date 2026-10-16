---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sobi.com
  spf: true
hosts:
- cert_expires: Mar 23 09:52:44 2027 GMT
  host: www.sobi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sobi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sobi (Swedish Orphan Biovitrum), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sobi (Swedish Orphan Biovitrum)
provider_slug: sobi
slug: sobi-domain-security
source_filename: sobi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sobi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 09:52:44 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sobi.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sobi/refs/heads/main/security/sobi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biopharma
- Rare Diseases
- Sweden
- Healthcare
---
